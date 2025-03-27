

Termux setup minimalist

create a syllabus for each apartado demtro de los apartados de la siguiente guia

y agrega indice symtaxys con hypervincylo 
**Guía Práctica para Termux: Instalación de Addons y Utilidades Esenciales (Copy & Paste)**

Esta guía te proporciona comandos listos para copiar y pegar directamente en tu terminal Termux.

**1. Configuración Inicial y Actualización:**

Antes de instalar cualquier cosa, es crucial actualizar y actualizar tu Termux.

```bash
pkg update && pkg upgrade -y
```

**2. Instalación de Addons de Termux:**

Los addons de Termux extienden la funcionalidad de Termux.

```bash
pkg install termux-api termux-boot termux-float termux-styling termux-tasker termux-widget -y
```

**Nota Importante:**

* `termux-api` requiere la instalación de la aplicación desde F-Droid o Google Play Store y otorgar permisos.
* `termux-tasker` requiere Tasker o una aplicación compatible.

**3. Instalación de Utilidades Base y Repositorios Adicionales:**

Estas utilidades son esenciales para un entorno de desarrollo y uso general.

```bash
pkg install x11-repo termux-x11-nightly tur-repo pulseaudio proot-distro wget git python python-pip python-dev openssh curl nano vim -y
```

**4. Configuración de Almacenamiento:**

Para acceder al almacenamiento de tu dispositivo.

```bash
termux-setup-storage
```

**5. Configuración de un Entorno de Escritorio X11 (Opcional):**

Para usar Termux como un entorno de escritorio.

```bash
pkg install xfce4 xfce4-terminal tigervnc xorg-server xterm lightdm xfwm4 xfce4-panel xfce4-settings xfce4-appfinder thunar firefox gedit lxterminal htop -y
```

**6. Inicio del Servidor VNC (Opcional, para Escritorio X11):**

```bash
vncserver :1 -geometry 1280x720 -depth 24
```

**Nota:** Se te pedirá que establezcas una contraseña para VNC.

**7. Inicio de XFCE (Opcional, para Escritorio X11):**

```bash
startxfce4 &
```

**8. Utilidades Adicionales:**

```bash
pkg install network-manager-applet pavucontrol -y
```

**Resumen de Comandos para Copiar y Pegar (Todo Junto):**

```bash
pkg update && pkg upgrade -y
pkg install termux-api termux-boot termux-float termux-styling termux-tasker termux-widget -y
pkg install x11-repo termux-x11-nightly tur-repo pulseaudio proot-distro wget git python python-pip python-dev openssh curl nano vim -y
termux-setup-storage
pkg install xfce4 xfce4-terminal tigervnc xorg-server xterm lightdm xfwm4 xfce4-panel xfce4-settings xfce4-appfinder thunar firefox gedit lxterminal htop -y
vncserver :1 -geometry 1280x720 -depth 24
startxfce4 &
pkg install network-manager-applet pavucontrol -y
```

**Instrucciones:**

1.  Abre Termux.
2.  Copia y pega cada bloque de comandos, uno a la vez, y presiona Enter.
3.  Sigue las indicaciones en pantalla (por ejemplo, otorgar permisos, establecer contraseñas).
4.  Para el entorno de escritorio X11, asegúrate de tener un cliente VNC en tu dispositivo para conectarte al servidor VNC.

**Notas Adicionales:**

* El uso de `-y` en los comandos de `pkg install` acepta automáticamente las instalaciones, lo que facilita el proceso.
* Ajusta las resoluciones y configuraciones según tus preferencias y las capacidades de tu dispositivo.
* Recuerda que algunos paquetes pueden requerir configuraciones adicionales después de la instalación.
* Para usar termux-api debes de instalar la app desde la tienda de F-droid o Google Play store, y darle los permisos correspondientes.



------------------------------------


<p align="center"><b style="font-size: xx-large">Easily Install Termux GUI Desktop</b></p>

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/sabamdarif/termux-desktop?style=for-the-badge) ![GitHub forks](https://img.shields.io/github/forks/sabamdarif/termux-desktop?color=teal&style=for-the-badge) ![GitHub issues](https://img.shields.io/github/issues/sabamdarif/termux-desktop?color=violet&style=for-the-badge) ![GitHub repo size](https://img.shields.io/github/repo-size/sabamdarif/termux-desktop?style=for-the-badge) ![GitHub License](https://img.shields.io/github/license/sabamdarif/termux-desktop?style=for-the-badge)

</div>


---

curl -Lf https://raw.githubusercontent.com/sabamdarif/termux-desktop/main/setup-termux-desktop -o setup-termux-desktop && chmod +x setup-termux-desktop && ./setup-termux-desktop



> **Note:** If you are in android 12 or higher then first disable *Phantom Process Killer* **Guide:-** [Here](https://github.com/atamshkai/Phantom-Process-Killer)
   ```bash
   curl -Lf https://raw.githubusercontent.com/sabamdarif/termux-desktop/main/setup-termux-desktop -o setup-termux-desktop && chmod +x setup-termux-desktop && ./setup-termux-desktop
   ```

##### If you select only one of them to access gui
- `gui --start / gui -l` *to start Termux gui*
- `gui --stop / gui -s` *to stop gui*





---------------------------



TERMUX NETHUNTER



termux-setup-storage
pkg install wget
wget -O install-nethunter-termux https://offs.ec/2MceZWr
chmod +x install-nethunter-termux
./install-nethunter-termux


pkg update -y && pkg upgrade -y 

sudo apt install tigervnc-standalone-server dbus-x11

sudo apt install kali-desktop-xfce

nethunter	
nethunter kex &	
sudo apt update && sudo apt full-upgrade -y

sudo apt install -y kali-linux-default

-------


Extras code server 


you use the install script, you can preview what occurs during the install process:

curl -fsSL https://code-server.dev/install.sh | sh -s -- --dry-run
To install, run:

curl -fsSL https://code-server.dev/install.sh | sh
When done, the install script prints out instructions for running and starting code-server.
