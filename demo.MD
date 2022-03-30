home assisant project-Play audio on a Bluetooth speaker with Raspberry Pi3b+
========

``single room Bluetooth speaker  with Raspberry Pi3b+`` — home assisant project.

Table of Contents
-----------------

  * [Introduce](#envirius)
    * [Introducing Bluez5](https://blog.csdn.net/Archer1991/article/details/62233164)
    * [Bluez vs ALSA  vs bluez-alsa vs PulseAudio vs home assisant media player](https://zhuanlan.zhihu.com/p/487809142?)
  * [Success Case](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3694)
    * [Start Bluetooth service on Debug Mode for error Message log](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3701)
    * [Check available versions for each plugin](#check-available-versions-for-each-plugin)
    * [Create an environment](#create-an-environment)
    * [Activate/deactivate environment](#activatedeactivate-environment
      * [Activating in the same shell](#activating-in-the-same-shell)
    * [Get list of environments](#get-list-of-environments)
    * [Get current activated environment](#get-current-activated-environment)
    * [Do something in environment without enabling it](#do-something-in-environment-without-enabling-it)
    * [Export environment into tar archive](#export-environment-into-tar-archive)
    * [Import environment from tar archive ](#import-environment-from-tar-archive)
    * [Get help](#get-help)
    * [Get help for a command](#get-help-for-a-command)
  * [Installation](#installation)
  * [Uninstallation](#uninstallation)
  * [Available plugins](#available-plugins)
  * [Bluetooth service](#usage)
    * [Start Bluetooth service on Debug Mode for error Message log](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3701)
    * [Check available versions for each plugin](#check-available-versions-for-each-plugin)
    * [Create an environment](#create-an-environment)
    * [Activate/deactivate environment](#activatedeactivate-environment
      * [Activating in the same shell](#activating-in-the-same-shell)
    * [Get list of environments](#get-list-of-environments)
    * [Get current activated environment](#get-current-activated-environment)
    * [Do something in environment without enabling it](#do-something-in-environment-without-enabling-it)
    * [Export environment into tar archive](#export-environment-into-tar-archive)
    * [Import environment from tar archive ](#import-environment-from-tar-archive)
    * [Get help](#get-help)
    * [Get help for a command](#get-help-for-a-command)
  * [Bluetooth Adapter Ready?](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3697)
    * [use rfkill to find out whether your computer has detected the installed Bluetooth hardware of your computer.](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3698)
      * [Bluetooth Adapter be blocked on your computer？](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3699)
      * [plug_url_for_download](#plug_url_for_download)
      * [plug_build](#plug_build)
    * [Software Configure ok?](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3705)
      * [hciconfig -a](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3708)
      * [show?](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3707)
    * [Examples](#examples)
  * [Bluetooth Connect Ready?](#3697)
    * [1.](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3698)
      * [Bluetooth Adapter be blocked on your computer？](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3699)
      * [plug_url_for_download](#plug_url_for_download)
      * [plug_build](#plug_build)
    * [Optional elements](#optional-elements)
      * [bluetooth speaker connect？](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/4#3738)
      * [Functions](#functions)
    * [Examples](#examples)
  * [PulseAudio](#3697)
    * [Install PulseAudio to get paplay pulseaudio、pactl、pacmd](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3710)
      * [Paired bluetooth speaker is not listed as an audio device](#3699)
      * [Use "pactl list cards" check bluez_card.9A_07_65_B4_21_EC exist or not](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3711)
      * [Use "pacmd list cards" check bluez_card.9A_07_65_B4_21_EC exist or not](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/3#3714)
    * [1](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3711)
      * [How to use PulseAudio set default audio to bluetooth speaker](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/3#3716)
      * [Functions](#functions)
    * [Examples](#examples)
   * [Bluetooth Adapter Ready?](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3697)
  * [trouble](#3698)
      * [Error when trying to connect to bluetooth speaker: `org.bluez.Error.Failed`](https://unix.stackexchange.com/questions/258074/error-when-trying-to-connect-to-bluetooth-speaker-org-bluez-error-failed)
      * [Error when trying to connect to bluetooth speaker:Failed to connect: org.bluez.Error.Failed br-connection-unknown](https://wonkodv.github.io/bluetooth-error/)
      * [plug_build](#plug_build)
    * [Optional elements](#optional-elements)
      * [[SOLVED]remove EA:AE:C8:B0:5E:88 Failed to remove device: org.bluez.Error.NotReady](https://www.msly.cn/boards/topic/3206/%E6%A0%91%E8%8E%93%E6%B4%BE%E9%80%9A%E8%BF%87linux%E4%B8%AD%E8%93%9D%E7%89%99%E5%8D%8F%E8%AE%AE%E6%A0%88bluz%E8%BF%9E%E6%8E%A5%E8%93%9D%E7%89%99%E9%9F%B3%E7%AE%B1%E6%8E%A5%E5%85%A5home-assistnant#3667)
      * [busctl tree org.bluez？](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3708)
      * [Functions](#functions)
    * [systemctl status bluetooth.service error](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/5#3742)
      * [[SOLVED]raspberrypi bluetoothd[420]: Failed to set mode: Blocked through rfkill (0x12)](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/5#3742)
      * [1](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3708)
      * [1](#functions)
    * [Examples](#examples)
  * [How to Set Your Wireless Bluetooth Speaker As the Default](#example-of-the-usage)
  * [Dependencies](#dependencies)
  * [Supported OS](#supported-os)
  * [Tests](#tests)
  * [Version History](#version-history)
  * [License](#license)
  * [README in another language](#readme-in-another-language)

Idea
----

Usually this kind of tools narrowly specialized for a particular
programming language. For example:

  * [virtualenv](https://github.com/pypa/virtualenv/) for python
  * [rvm](https://github.com/wayneeseguin/rvm/) for ruby
  * [kerl](https://github.com/spawngrid/kerl/) for erlang
  * [nvm](https://github.com/creationix/nvm)/[nodeenv](https://github.com/ekalinin/nodeenv/) for node.js
  * and so on

But there are many cases when in the same environment you must have more
than one programming language. For example, to create an environment with
``python2.6`` and ``node.js 0.10.24``. This idea underlies ``envirius``.

Support for new programming languages are implemented as plug-ins (see below).

Features
--------

* clean design
* easy extensible
* test coverage

Installation
============

At first:

```bash
$ git clone https://github.com/ekalinin/envirius.git
$ cd envirius
$ make install
```

Then youd need to add into your ``.bashrc`` the following:

```bash
[ -f "$HOME/.envirius/nv" ] && . ~/.envirius/nv
```

Uninstallation
==============

Just do the following:

```bash
$ cd envirius
$ make uninstall
```

Cache and previously created environments will not be deleted.

Available plugins
=================

You can create environments for the following programming languages:

* [erlang](http://erlang.org/)
* [rust](http://rust-lang.org/)
* [elixir](http://elixir-lang.org/)
* [julia](http://julialang.org/)
* [node.js](http://nodejs.org/)
* [iojs](https://iojs.org/)
* [python](https://www.python.org/)
* [go](http://golang.org/)
* [haskell](http://haskell.org/)
* [scala](http://scala-lang.org/)

New languages can be added as plugins (see below).

Usage
=====

Check available plugins
-----------------------

```bash
➥ nv ls-plugins
elixir
elixir-prebuilt
erlang
go-prebuilt
haskell
haskell-prebuilt
iojs
iojs-prebuilt
julia
node
node-prebuilt
python
rust
rust-prebuilt
scala
