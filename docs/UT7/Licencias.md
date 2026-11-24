# 7.1 Clasificación y licencias de software

## 1. Clasificación del software

El software se puede clasificar según su finalidad en tres grandes grupos:

- **Software de sistema:** administra los componentes físicos del ordenador y permite que funcionen otros programas. Ejemplos: Windows, GNU/Linux y los controladores.
- **Software de programación:** incluye herramientas utilizadas para desarrollar aplicaciones, como Visual Studio Code, Python o compiladores.
- **Software de aplicación:** permite realizar tareas específicas, como navegar por Internet, editar documentos, diseñar imágenes o gestionar una empresa.

## 2. Licencias de software

Una licencia de software es un contrato legal que establece las condiciones de uso de un programa. Determina si podemos instalarlo, copiarlo, modificarlo o distribuirlo.

Es importante diferenciar entre software libre y software gratuito:

- **Software libre:** permite utilizar, estudiar, modificar y distribuir el programa.
- **Freeware:** es gratuito, pero normalmente tiene código cerrado y restricciones de uso.
- **Software propietario:** limita las modificaciones y la distribución del programa.

### Las cuatro libertades del software libre

1. Libertad 0: utilizar el programa para cualquier propósito.
2. Libertad 1: estudiar cómo funciona y modificarlo.
3. Libertad 2: distribuir copias.
4. Libertad 3: mejorar el programa y compartir las mejoras.

## 3. Tipos de licencias

| Tipo de licencia | Características | Ejemplos |
|---|---|---|
| Propietaria | Código cerrado y uso restringido. | Windows, Photoshop |
| Shareware | Permite probar el programa durante un tiempo limitado. | WinRAR |
| Freeware | Uso gratuito, pero código cerrado. | Google Chrome |
| GPL | Software libre con obligación de mantener la licencia en obras derivadas distribuidas. | Linux, GIMP |
| LGPL | Permite utilizar bibliotecas libres desde programas con otras licencias. | glibc |
| MIT / BSD / Apache | Licencias permisivas que permiten reutilizar y modificar el código. | Node.js |
| Dominio público / CC0 | Permite reutilizar el contenido sin derechos exclusivos de explotación. | SQLite |

## 4. Licencias Creative Commons

Las licencias Creative Commons se utilizan principalmente para compartir contenidos creativos, como fotografías, vídeos, documentos y textos.

Sus principales condiciones son:

- **BY:** reconocer la autoría.
- **SA:** compartir las modificaciones con la misma licencia.
- **NC:** prohibir el uso comercial.
- **ND:** prohibir la distribución de obras modificadas.

| Licencia | Uso comercial | Permite modificaciones |
|---|---|---|
| CC BY | Sí | Sí |
| CC BY-SA | Sí | Sí |
| CC BY-NC | No | Sí |
| CC BY-ND | Sí | No |
| CC BY-NC-SA | No | Sí |
| CC0 | Sí | Sí |

## 5. Comprobación de licencias

Podemos consultar la información de las licencias de los programas mediante comandos del sistema operativo.

**Ejemplo en Windows PowerShell:**

```powershell
# Consultar información de VLC
winget show VideoLAN.VLC

# Consultar información de 7-Zip
winget show 7zip.7zip
```

En Linux también podemos consultar los paquetes instalados y sus licencias:

```bash
# Consultar información del paquete Git
dpkg -s git

# Consultar su información de licencia
cat /usr/share/doc/git/copyright
```

> [!TIP]
> Antes de instalar o utilizar un programa, es recomendable comprobar su licencia para conocer qué permisos tenemos y qué restricciones debemos respetar.

## 6. Conclusión

Las licencias de software son importantes porque establecen los derechos y obligaciones de los usuarios y desarrolladores. Conocer los diferentes tipos de software y sus licencias permite elegir los programas adecuados y utilizarlos de forma legal y responsable.