home assisant project-remote access on Raspberry Pi3b+
========

``remote access on Raspberry Pi3b+`` — home assisant project.

Table of Contents
-----------------

  * [Install](#envirius)
    * [buy a domain](https://blog.csdn.net/Archer1991/article/details/62233164)
    * [buy a vps](https://zhuanlan.zhihu.com/p/487809142?)
  * [Install](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3694)
    * [Install frp](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3701)
    * [Install py](#check-available-versions-for-each-plugin)
    * [Install home assisant](#create-an-environment)
    * [Install nginx](#activatedeactivate-environment)
      * [https](#activating-in-the-same-shell)
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
 
