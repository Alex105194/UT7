# 7.5 Transferencia de ficheros

## 1. Métodos de transferencia

La transferencia de ficheros consiste en enviar archivos entre dispositivos. Se puede realizar mediante USB, Bluetooth, correo electrónico, almacenamiento en la nube o servidores remotos.

| Método | Ejemplo | Uso |
|---|---|---|
| USB | Pendrive | Transferencia local |
| Nube | Google Drive | Compartir archivos |
| Correo | Gmail | Enviar documentos |
| FTP/SFTP | FileZilla | Transferencia a servidores |
| Red local | SMB | Compartir carpetas |

## 2. Protocolos de transferencia

Los protocolos establecen cómo se envían los archivos entre equipos.

| Protocolo | Puerto | Característica |
|---|---|---|
| FTP | 21 | No cifra los datos |
| FTPS | 21/990 | Utiliza TLS |
| SFTP | 22 | Utiliza SSH |
| SCP | 22 | Copia archivos mediante SSH |
| TFTP | 69 | Transferencia sencilla |

> [!WARNING]
> FTP no cifra las contraseñas ni los datos. Es preferible utilizar SFTP o FTPS para realizar transferencias seguras.

## 3. Programas de transferencia

Algunos programas permiten gestionar archivos de forma sencilla:

- **FileZilla:** permite transferir archivos mediante FTP, FTPS y SFTP.
- **WinSCP:** permite realizar transferencias seguras en Windows.
- **SCP y SFTP:** permiten enviar y recibir archivos desde la terminal.

## 4. Ejemplo práctico

Podemos utilizar SCP para enviar un archivo a un servidor remoto:

```bash
# Enviar un archivo al servidor
scp documento.pdf usuario@192.168.1.50:/home/usuario/

# Conectarse mediante SFTP
sftp usuario@192.168.1.50
```

> [!TIP]
> Utiliza SFTP o SCP cuando necesites transferir archivos de forma segura mediante SSH.

## 5. Seguridad

Para proteger los archivos compartidos debemos:

- Utilizar conexiones cifradas.
- Establecer contraseñas seguras.
- Controlar los permisos de acceso.
- Evitar enlaces públicos con información privada.
- Compartir archivos solo con personas autorizadas.

## 6. Conclusión

La transferencia de ficheros permite compartir información entre dispositivos. Es importante conocer los protocolos disponibles y utilizar herramientas seguras como SFTP, SCP o FTPS para proteger los datos.