# 7.1 Clasificación y licencias de software

Antes de instalar o recomendar un programa conviene saber para qué sirve (su propósito) y qué permite hacer legalmente (su licencia).

## 1. Clasificación según su propósito
| Tipo | Función | Ejemplos |
|------|---------|----------|
| Software de sistema | Gestiona el hardware y sirve de base al resto | Windows, GNU/Linux, controladores, UEFI/BIOS |
| Software de programación | Crear, compilar, interpretar y depurar aplicaciones | VS Code, gcc, Python |
| Software de aplicación | Resuelve tareas concretas del usuario o empresa | Ofimática, navegadores, ERP |

## 2. Licencias de software
Una licencia es el contrato legal que fija qué puede hacer el usuario con el programa. Define derechos (instalar, copiar, modificar, redistribuir), protege la autoría y evita problemas legales.

> [!WARNING]
> Libre no significa gratuito. El software libre se refiere a las libertades del usuario y puede venderse. El software gratuito (freeware) suele ser propietario y de código cerrado.

### Las cuatro libertades del software libre
| Libertad | Qué permite |
|----------|-------------|
| 0 | Ejecutar el programa con cualquier propósito |
| 1 | Estudiar cómo funciona y cambiarlo (requiere el código fuente) |
| 2 | Redistribuir copias para ayudar a otros |
| 3 | Distribuir copias de las versiones modificadas |

### Espectro de licencias
| Modelo | Código | Modificación y redistribución | Ejemplos |
|--------|--------|-------------------------------|----------|
| Privativo | No | Prohibidas sin permiso | Windows, Microsoft Office |
| Shareware / Trial | No | Prueba gratuita limitada | WinRAR |
| Freeware | No | Uso gratuito, código cerrado | Google Chrome, Adobe Acrobat Reader |
| Libre copyleft fuerte (GPL) | Sí | Permitidas; las obras derivadas mantienen la GPL | Kernel Linux, GIMP |
| Libre copyleft débil (LGPL, MPL) | Sí | Integrables con software privativo | LibreOffice, Thunderbird |
| Libre permisivo (MIT, BSD, Apache) | Sí | Permitidas citando la autoría | Node.js, Apache HTTP Server |
| Dominio público / CC0 | Sí | Sin derechos exclusivos vigentes | SQLite |

## 3. Comprobación práctica de licencias
En Windows (PowerShell), se puede consultar la licencia de un paquete con winget:

```powershell
winget show VideoLAN.VLC
winget show 7zip.7zip
```

> [!TIP]
> En Linux (Debian/Ubuntu) se consulta con `dpkg -s git` y con `cat /usr/share/doc/git/copyright | head -n 20`.