home assisant project-Play audio on a Bluetooth speaker with Raspberry Pi3b+
========

``single room Bluetooth speaker  with Raspberry Pi3b+`` — home assisant project.

Table of Contents
-----------------

  * [Introduce](#envirius)
    * [Introducing Bluez5](#idea)
    * [Bluez vs ALSA  vs bluez-alsa vs PulseAudio vs home assisant media player](https://zhuanlan.zhihu.com/p/487809142?)
  * [Installation](#installation)
  * [Uninstallation](#uninstallation)
  * [Available plugins](#available-plugins)
  * [Usage](#usage)
    * [Check available plugins](#check-available-plugins)
    * [Check available versions for each plugin](#check-available-versions-for-each-plugin)
    * [Create an environment](#create-an-environment)
    * [Activate/deactivate environment](#activatedeactivate-environment)
      * [[SOLVED]Failed to remove device: org.bluez.Error.NotReady](https://www.msly.cn/boards/topic/3206/%E6%A0%91%E8%8E%93%E6%B4%BE%E9%80%9A%E8%BF%87linux%E4%B8%AD%E8%93%9D%E7%89%99%E5%8D%8F%E8%AE%AE%E6%A0%88bluz%E8%BF%9E%E6%8E%A5%E8%93%9D%E7%89%99%E9%9F%B3%E7%AE%B1%E6%8E%A5%E5%85%A5home-assistnant#3667)
      * [Activating in the same shell](#activating-in-the-same-shell)
    * [Get list of environments](#get-list-of-environments)
    * [Get current activated environment](#get-current-activated-environment)
    * [Do something in environment without enabling it](#do-something-in-environment-without-enabling-it)
    * [Export environment into tar archive](#export-environment-into-tar-archive)
    * [Import environment from tar archive ](#import-environment-from-tar-archive)
    * [Get help](#get-help)
    * [Get help for a command](#get-help-for-a-command)
  * [How to add a plugin?](#how-to-add-a-plugin)
    * [Mandatory elements](#mandatory-elements)
      * [plug_list_versions](#plug_list_versions)
      * [plug_url_for_download](#plug_url_for_download)
      * [plug_build](#plug_build)
    * [Optional elements](#optional-elements)
      * [Variables](#variables)
      * [Functions](#functions)
    * [Examples](#examples)
  * [Example of the usage](#example-of-the-usage)
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
