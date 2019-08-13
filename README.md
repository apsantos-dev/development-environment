# Development Environment - FEDORA 30

## Introduction

The main objective of this project is to share some tools used in everyday life for the development of web and mobile applications.

<!-- Badges section here. -->
[![License][license-img]][license-ln]
[![CONTRIBUTING][contributing-img]][contributing-ln]
[![GitHub stars][github-stars-img]][github-stars-ln]
[![GitHub forks][github-forks-img]][github-forks-ln]
[![Twitter Follow][twitter-follow-img]][twitter-follow-ln]

---

### Before You Begin

The development of this project was done in environment [Linux][linux-ln], using the Operating System [Fedora 30][fedora-ln]. I used [Terminal][terminal-ln] to run the [commands][commands-ln] described in this tutorial.

```sh
lsb_release -a  # to check system details
```

When it is necessary to execute a command as [root][root-ln], I'll describe the content as follows. Example:

```sh
sudo dnf install xyz  # command example
```

I recommend that you use the Operating System of your choice, adapting the project according to system standards.

> Additional | Editor:
>
> [VSCode][vscode-ln]: Visual Studio Code is a lightweight but powerful source code editor. \o/

### VSCode version on my machine

> Version: 1.37.0 \
Commit: 036a6b1d3ac84e5ca96a17a44e63a87971f8fcc8 \
Date: 2019-08-08T01:24:14.598Z \
Electron: 4.2.7 \
Chrome: 69.0.3497.128 \
Node.js: 10.11.0 \
V8: 6.9.427.31-electron.0 \
OS: Linux x64 5.2.6-200.fc30.x86_64

## Getting Started

### Installation

1 - To execute this project, I recommend that you have some tools installed on your machine. Are they:

- [VSCode][vscode-ln]: Visual Studio Code on Linux - RHEL, Fedora and CentOS based distributions

  ```sh
  sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc

  sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'
  ```

  Then update the package cache and install the package using dnf (Fedora 22 and above):

  ```sh
  dnf check-update
  sudo dnf install code
  ```

  _For details on installing extension in VSCode, visit the following website: [VSCode Install][vscode-in]_

---

- [Git][git-ln]: Git is a free and open source distributed version control system.

  ```sh
  git --version  # to print Git version
  ```

  If you need to install Git, use the command:

  ```sh
  sudo dnf install git -y   # to install Git on your operating system
  ```

2 - Clone the project:

```sh
cd ~  # open folder for project creation
git clone git@github.com:apsantos-dev/development-environment.git <NAME-PROJECT>  # SSH

or

git clone https://github.com/apsantos-dev/development-environment.git <NAME-PROJECT> # HTTPS

```

_See this [file][ssh-file] for details on how to use [SSH][ssh-ln] in your project._

3 - Attributes and permissions:

Change the attributes and permissions of the file: [apsantos.sh](apsantos.sh "Click to open the project")

> Be sure to check in which folder this project was cloned.

```sh
sudo chown $USER:$USER ~/<NAME-PROJECT>/apsantos.sh
sudo chmod +x ~/<NAME-PROJECT>/apsantos.sh
```

4 - Finally, running the system:

If all the steps have been performed correctly, just execute the command below to start the system:

```sh
sh ~/<NAME-PROJECT>/apsantos.sh
```

_There are several ways to do this, however,
we will limit ourselves to this =]_

### Installed Programs

See in [this file][installedPrograms] some of the programs used in my daily life.

### Structure

See the file and folder [structure][structure-ln] for this project.

### Visual Studio Code Extensions

[Click here][extensions-ln] to open the file with the extensions used.

### Change Log

All notable changes to this project will be documented in the file [CHANGELOG.md][changelog-ln].

_Stable release version:_

[![Release][release-img]][release-ln]

### Contributing

By contributing to this repository, please first discuss the change you wish to make via email or any other method with the owners of this repository before making a change.

_See details on contributing to this project at:_

[![CONTRIBUTING][contributing-img]][contributing-ln]

### License

This project is licensed under "[The MIT License (MIT)][mit-ln]".

_See license details at:_

[![License][license-img]][license-ln]

<!-- links -->
[changelog-ln]: CHANGELOG.md "Click here to open the file"
[commands-ln]: https://en.wikipedia.org/wiki/Command_(computing) "Press Ctrl and click this link to open the page in a new tab"
[contributing-img]: https://img.shields.io/badge/development&ndash;environment-CONTRIBUTE-orange.svg?style=flat-square
[contributing-ln]: CONTRIBUTING.md "Contribute to make this boilerplate even better"
[extensions-ln]: src/assets/doc/extensions.md "Click here to open the file"
[fedora-ln]: https://getfedora.org/en/ "Press Ctrl and click this link to open the page in a new tab"
[git-ln]: https://git-scm.com/ "Press Ctrl and click this link to open the page in a new tab"
[github-stars-img]: https://img.shields.io/github/stars/apsantos-dev/development-environment.svg?style=social&label=Star
[github-stars-ln]: https://github.com/apsantos-dev/development-environment/stargazers "See who likes this design = ]"
[github-forks-img]: https://img.shields.io/github/forks/apsantos-dev/tests.svg?style=social&label=Fork
[github-forks-ln]: https://github.com/apsantos-dev/development-environment/fork "Click to view Star details of this project"
[installedPrograms]: src/assets/doc/installed-programs.md "Click here to open the file"
[license-img]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-ln]: LICENSE "Copyright (c) 2019 APSantos Desenvolvimento de Sistemas"
[linux-ln]: https://en.wikipedia.org/wiki/Linux "Press Ctrl and click this link to open the page in a new tab"
[mit-ln]: https://opensource.org/licenses/MIT "Click and see the project"
[release-img]: https://img.shields.io/github/release/apsantos-dev/development-environment.svg?style=flat-square
[release-ln]: https://github.com/apsantos-dev/development-environment/releases "See all versions of this project"
[root-ln]: https://en.wikipedia.org/wiki/Sudo "Press Ctrl and click this link to open the page in a new tab"
[structure-ln]: structure.md "Click and see the project!"
[ssh-file]: src/assets/doc/ssh.md "Click here to open the file"
[ssh-ln]: https://pt.wikipedia.org/wiki/Secure_Shell "Press Ctrl and click this link to open the page in a new tab"
[terminal-ln]: https://en.wikipedia.org/wiki/Linux_console "Press Ctrl and click this link to open the page in a new tab"
[twitter-follow-img]: https://img.shields.io/twitter/follow/apsantos_dev.svg?label=Follow&style=social
[twitter-follow-ln]: https://twitter.com/intent/follow?screen_name=apsantos_dev "View my profile on Twitter"
[vscode-ln]: https://code.visualstudio.com/ "Press Ctrl and click this link to open the page in a new tab"
[vscode-in]: https://code.visualstudio.com/docs/setup/linux#_rhel-fedora-and-centos-based-distributions "Press Ctrl and click this link to open the page in a new tab"
