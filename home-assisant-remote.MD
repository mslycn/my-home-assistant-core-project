home assisant project-remote access on Raspberry Pi3b+
========

``remote access on Raspberry Pi3b+`` — home assisant project.

Table of Contents
-----------------

  * [Install](#envirius)
    * [buy a domain](https://blog.csdn.net/Archer1991/article/details/62233164)
    * [buy a vps](https://zhuanlan.zhihu.com/p/487809142?)
  * [Install nginx on vps](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3694)
    * [Install nginx](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3701)
    * [test use domain visit nginx web server](#check-available-versions-for-each-plugin)
    * [Install home assisant](#create-an-environment)
    * [Install nginx](#activatedeactivate-environment)
      * [https](#activating-in-the-same-shell)
  * [Install frp](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3694)
    * [Install frp server on vps](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3701)
    * [Install frp client on pi](#check-available-versions-for-each-plugin)
      * [https](#activating-in-the-same-shell)
  * [trouble-Access to HA via chrome browser is not OK](#3698)
      * [Set home assisant logger level for debug](https://www.home-assistant.io/integrations/logger/)
      * [2](https://wonkodv.github.io/bluetooth-error/)
      * [3](#plug_build)
    * [login failure](#optional-elements)
      * [Unable to connect to Home Assistant. RETRY](https://www.msly.cn/boards/topic/3227/home-assistant-remote-access-test-step-by-step#3822)
      * [1](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3708)
      * [1](#functions)
    * [systemctl status bluetooth.service error](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/5#3742)
      * [1](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/5#3742)
      * [1](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist/page/2#3708)
      * [1](#functions)
  * [expose http server](https://www.msly.cn/boards/topic/34/home-assistant-remote-access-solution/page/2#3746)
    * [Make core listen on:0.0.0.0.8153](https://www.msly.cn/boards/topic/34/home-assistant-remote-access-solution/page/2#3746)
    * [Make http accept in comming ip address](https://www.msly.cn/boards/topic/34/home-assistant-remote-access-solution/page/2#3758)
      * [https](#activating-in-the-same-shell)

 
