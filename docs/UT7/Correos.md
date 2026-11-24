# 7.4 Correo y mensajería electrónica

## 1. Correo electrónico y mensajería instantánea

En los entornos profesionales existen dos formas principales de comunicación digital: el correo electrónico y la mensajería instantánea.

- **Correo electrónico:** es un medio de comunicación asíncrono, es decir, no requiere que el destinatario responda inmediatamente. Permite enviar mensajes formales, documentos y archivos adjuntos.
- **Mensajería instantánea:** permite comunicarse en tiempo real mediante chats, canales y llamadas. Es útil para coordinar tareas y trabajar en equipo.

| Característica | Correo electrónico | Mensajería instantánea |
|---|---|---|
| Comunicación | Asíncrona | Síncrona |
| Velocidad | No inmediata | Inmediata |
| Uso principal | Comunicación formal | Coordinación rápida |
| Archivos | Archivos adjuntos | Compartir archivos |
| Ejemplos | Gmail, Outlook | WhatsApp, Teams, Slack |

## 2. Protocolos del correo electrónico

El correo electrónico utiliza diferentes protocolos para enviar, recibir y almacenar mensajes.

- **SMTP:** se encarga del envío de correos electrónicos.
- **IMAP:** permite consultar y sincronizar los mensajes directamente con el servidor.
- **POP3:** descarga los mensajes al dispositivo local, pudiendo eliminarlos del servidor según su configuración.

### Puertos principales

| Protocolo | Puerto | Seguridad | Función |
|---|---|---|---|
| SMTP | 587 | STARTTLS | Envío de correos |
| SMTP | 465 | TLS | Envío cifrado |
| IMAP | 993 | SSL/TLS | Recepción y sincronización |
| POP3 | 995 | SSL/TLS | Descarga de mensajes |
| SMTP | 25 | Depende de configuración | Comunicación entre servidores |

Es recomendable utilizar conexiones cifradas para proteger la información transmitida.

> [!NOTE]
> IMAP es especialmente útil cuando utilizamos varios dispositivos, ya que mantiene los correos sincronizados con el servidor.

## 3. Clientes de correo electrónico

Los clientes de correo permiten gestionar nuestros mensajes, organizar la bandeja de entrada y enviar archivos.

Existen dos modalidades:

- **Webmail:** permite acceder al correo desde un navegador sin instalar programas. Ejemplos: Gmail, Outlook.com y Proton Mail.
- **Clientes de escritorio o móvil:** son aplicaciones instaladas en el dispositivo. Ejemplos: Mozilla Thunderbird, Microsoft Outlook y Evolution.

### Organización del correo

Los mensajes pueden organizarse mediante carpetas o etiquetas.

- Las carpetas permiten clasificar los mensajes en diferentes ubicaciones.
- Las etiquetas permiten asignar varias categorías a un mismo correo, como sucede en Gmail.

## 4. Destinatarios: Para, CC y CCO

Al enviar un correo podemos utilizar diferentes campos para indicar quién recibe el mensaje.

| Campo | Significado | Función |
|---|---|---|
| Para | Destinatario principal | Persona que debe recibir y atender el mensaje |
| CC | Copia de carbón | Personas que deben estar informadas |
| CCO | Copia de carbón oculta | Destinatarios cuyas direcciones permanecen ocultas |

### Privacidad y RGPD

Cuando enviamos un correo a varias personas externas, debemos utilizar CCO para evitar que los destinatarios conozcan las direcciones de correo de los demás.

> [!WARNING]
> No utilices el campo Para o CC para enviar mensajes masivos a personas externas si no tienen autorización para conocer las direcciones del resto.

## 5. Comprobación de conectividad

Es posible comprobar si los puertos utilizados por los servidores de correo están accesibles desde nuestro ordenador.

### En Windows (PowerShell)

```powershell
# Comprobar conexión SMTP
Test-NetConnection smtp.office365.com -Port 587

# Comprobar conexión IMAP
Test-NetConnection outlook.office365.com -Port 993
```

### En Linux

```bash
# Comprobar si el puerto SMTP está abierto
nc -zv smtp.office365.com 587

# Comprobar conexión segura IMAP
openssl s_client -connect outlook.office365.com:993 -brief
```

Estos comandos ayudan a detectar problemas de conexión con los servidores de correo.

## 6. Mensajería instantánea y colaboración

Las herramientas de mensajería permiten mejorar la comunicación y el trabajo colaborativo.

| Aplicación | Características | Uso habitual |
|---|---|---|
| Microsoft Teams | Integración con Microsoft 365 | Entornos empresariales |
| Slack | Canales, bots e integraciones | Equipos de desarrollo |
| Google Chat | Integración con Google Workspace | Trabajo colaborativo |
| Discord | Servidores y canales | Comunidades técnicas |
| Telegram | Bots y envío de archivos | Comunicación general |
| WhatsApp | Mensajes y llamadas | Comunicación cotidiana |
| Signal | Cifrado de extremo a extremo por defecto | Privacidad |

### Seguridad en la mensajería

Es importante utilizar correctamente estas herramientas para proteger la información.

- No enviar contraseñas en texto plano.
- Evitar compartir información confidencial mediante cuentas personales.
- Utilizar los canales corporativos autorizados.
- Comprobar la identidad de los destinatarios.
- Utilizar aplicaciones con medidas de seguridad adecuadas.

> [!TIP]
> Para trabajar en equipo es recomendable utilizar herramientas como Teams o Slack, ya que permiten organizar conversaciones por canales y compartir información de forma ordenada.

## 7. Conclusión

El correo electrónico y la mensajería instantánea son herramientas fundamentales en cualquier entorno profesional.

El correo electrónico resulta más adecuado para comunicaciones formales y documentos, mientras que la mensajería instantánea facilita la colaboración en tiempo real.

También es importante conocer los protocolos SMTP, IMAP y POP3, utilizar conexiones cifradas y respetar la privacidad de los destinatarios para mantener una comunicación segura y eficiente.