# Installed Programs

The purpose of this file is to demonstrate through the [Terminal][terminal-ln] how to install some of the tools used to develop web and mobile systems.

Not all programs mentioned here are required to use [sudo](https://pt.wikipedia.org/wiki/Sudo) command. Are they:

`Soon, I will leave my considerations on each program used. =]`

> _The following commands were used in [Terminal][terminal-ln] using [Bash][bash]_

---

## Angular CLI

CLI Overview and Command Reference.

> The Angular CLI is a command-line interface tool that you use to initialize, develop, scaffold, and maintain Angular applications. You can use the tool directly in a command shell, or indirectly through an interactive UI such as Angular Console.

_[Details on this link!](https://angular.io/cli)_

**_Install_**:

```sh
sudo npm install -g @angular/cli
```

**_Use_**:

> _`A tutorial on this item will be available soon.`_

---

## Cordova

Mobile apps with HTML, CSS & JS. Target multiple platforms with one code base. Free and open source.

_[Details on this link!](https://cordova.apache.org/docs/en/latest/)_

**_Install_**:

```sh
sudo npm install -g cordova
```

**_Use_**:

> _`A tutorial on this item will be available soon.`_

---

## Fedy

Fedy lets you install multimedia codecs and additional software that Fedora doesn’t want to ship, such as MP3 support, Adobe Flash, Oracle Java, and much more, with just a few clicks.

_[Details on this link!](https://www.folkswithhats.org/)_

**_Install_**:

```sh
sudo dnf install https://dl.folkswithhats.org/fedora/$(rpm -E %fedora)/RPMS/fedy-release.rpm

sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm

sudo dnf install fedy
```

**_Open_**:

```sh
fedy
```

---

## Firebase tools

Firebase CLI offers a number of management, visualization and deployment tools for Firebase projects.

_[Details on this link!](https://firebase.google.com/docs)_

**_Install_**:

```sh
sudo npm install -g firebase-tools
```

**_Open_**:

> _`A tutorial on this item will be available soon.`_

---

## Flameshot

Powerful yet simple to use screenshot software. Easy to use. Customizable appearance. In-app screenshot edit.

_[Details on this link!](https://flameshot.js.org/#/)_

**_Install_**:

```sh
sudo dnf install flameshot -y
```

**_Open_**:

```sh
flameshot gui
```

> Press ESC to close the program.

---

## Flash Player

Adobe® Flash® Player is a lightweight browser plug-in and runtime application with many Internet features that offers consistent and engaging user experiences, exceptional audio / video playback and exciting games.

_[Details on this link!](https://get.adobe.com/br/flashplayer/) or [Fedora Docs](https://docs.fedoraproject.org/en-US/quick-docs/using-adobe-flash/)_

**_Install_**:

```sh
sudo dnf makecache -y

sudo rpm -ivh http://linuxdownload.adobe.com/adobe-release/adobe-release-x86_64-1.0-1.noarch.rpm

sudo rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-adobe-linux

sudo dnf install flash-plugin alsa-plugins-pulseaudio libcurl -y
```

**_Open_**:

```sh
Firefox: about:plugins
Chrome: chrome://flash
```

---

## Gimp

GIMP is an acronym for GNU Image Manipulation Program. It is a freely distributed program for such tasks as photo retouching, image composition and image authoring. The terms of usage and rules about copying are clearly listed in the [GNU General Public License](https://www.gimp.org/about/COPYING). [There is a nice Frequently Asked Questions (FAQ)](https://www.gimp.org/docs/userfaq.html) page.

_[Details on this link!](https://www.gimp.org/about/)_

**_Install_**:

```sh
sudo dnf install gimp -y
```

**_Open_**:

```sh
gimp
```

---

## Git

Git is a [free and open source](https://git-scm.com/about/free-and-open-source) distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

_[Details on this link!](https://git-scm.com/)_

**_Install_**:

```sh
sudo dnf install git
```

**_Open_**:

> _`A tutorial on this item will be available soon.`_

---

## GNOME Tweaks

GNOME Tweaks allows adjusting advanced GNOME options.

> It can install and manage themes and extensions, change power settings, manage startup applications, and enable desktop icons among other settings.

_[Details on this link!](https://wiki.gnome.org/Apps/Tweaks)_

**_Install_**:

```sh
sudo dnf install gnome-tweak-tool
```

**_Open_**:

```sh
gnome-tweaks
```

---

## HTOP

htop is a process viewer and interactive process manager. It is designed as an alternative to the top Unix program. It shows an updated (often) list of processes running on a computer, usually sorted by the amount of CPU usage.

_[Details on this link!](https://pt.wikipedia.org/wiki/Htop)_

**_Install_**:

```sh
sudo dnf install htop -y
```

**_Open_**:

```sh
htop
```

> Press ESC to close the program.

---

## Ionic

One codebase. Any platform.

> Built on standard web technology, Ionic helps teams build and ship beautiful cross-platform hybrid and Progressive Web Apps with ease.

_[Details on this link!](https://ionicframework.com/)_

**_Install_**:

```sh
sudo npm install -g ionic
```

**_Open_**:

> _`A tutorial on this item will be available soon.`_

---

## NodeJS and NPM

As an asynchronous event driven JavaScript runtime, Node is designed to build scalable network applications. In the following "hello world" example, many connections can be handled concurrently. Upon each connection the callback is fired, but if there is no work to be done, Node will sleep.

_[Details on this link!](https://nodejs.org/en/about/)_

**_Install_**:

```sh
sudo dnf install gcc-c++ make -y

curl -sL https://rpm.nodesource.com/setup_12.x | sudo -E bash -

sudo dnf install nodejs -y
```

**_Details_**:

```sh
node --version
npm --version
```

---

## Skype

Skype is software that enables communication over the Internet through voice and video connections, created by Janus Friis and Niklas Zennstrom.

_[Details on this link!](https://www.skype.com/)_

**_Install_**:

```sh
cd /tmp

sudo dnf install wget -y

wget --trust-server-names https://go.skype.com/skypeforlinux-64.rpm

sudo dnf install /tmp/skypeforlinux-64.rpm -y
```

**_Open_**:

```sh
skypeforlinux
```

---

## Steam

Steam is digital rights management software created by Valve Corporation or Valve L.L.C., of digital platforms such as games and programming applications, and provide easy services like automatic game updating, and affordable pricing to users.

_[Details on this link!](https://store.steampowered.com/?l=portuguese)_

**_Install_**:

```sh
sudo dnf update --refresh

sudo dnf install steam -y
```

**_Open_**:

```sh
steam
```

---

## Teamview

TeamViewer is a proprietary software package for remote access, desktop sharing, online conferencing, and file transfer between computers. The program operates within the operating systems: Microsoft Windows, OS X, Linux, iOS, Android, Windows RT and Windows Phone.

_[Details on this link!](https://www.teamviewer.com)_

**_Install_**:

```sh
sudo dnf install wget -y

wget https://download.teamviewer.com/download/linux/teamviewer.x86_64.rpm

sudo dnf install teamviewer.x86_64.rpm -y
```

**_Open_**:

```sh
teamviewer
```

**_Details_**:

```sh
rpm -qi teamviewer
```

---

## Typescript

TypeScript is a superset of JavaScript developed by Microsoft that adds typing and some other features to the language. Anders Hejlsberg, architect of the C # language and creator of the Delphi and Turbo Pascal languages, worked on the development of TypeScript.

_[Details on this link!](https://www.typescriptlang.org/)_

**_Install_**:

```sh
sudo npm i -g typescrip
```

**_Open_**:

> _`A tutorial on this item will be available soon.`_

---

## Visual Studio Code

Visual Studio Code is a source code editor developed by Microsoft for Windows, Linux, and macOS. It includes support for debugging, embedded Git control, syntax highlighting, smart code completion, snippets, and code refactoring.

_[Details on this link!](https://code.visualstudio.com/)_

**_Install_**:

```sh
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc

sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'

dnf check-update

sudo dnf install code
```

**_Open_**:

```sh
code
```

---

## VLC

VLC media player is an open source multimedia player / player and transmitter. It supports various video formats such as OGM, MPEG1, MPEG-2, MPEG-4, DivX, Blu-ray, DVD, VCDs, etc. and audio such as OGG, Speex, FLAC, MPC, MP3, WAV and others.

_[Details on this link!](https://www.videolan.org/vlc/index.pt-BR.html)_

**_Install_**:

```sh
sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm -y

sudo dnf install vlc -y
```

**_Open_**:

```sh
vlc
```

---

<!-- links -->
[terminal-ln]: https://en.wikipedia.org/wiki/Linux_console "Press Ctrl and click this link to open the page in a new tab"
[bash]: https://pt.wikipedia.org/wiki/Bash "Press Ctrl and click this link to open the page in a new tab"
