home assisant project-install home assisant core 2022.3.0  on Raspberry Pi3b+
========

``install home assisant core 2022.3.0s on Raspberry Pi3b+`` — home assisant project.

Table of Contents
-----------------

  * [Install](#envirius)
    * [buy a domain](https://blog.csdn.net/Archer1991/article/details/62233164)
    * [buy a vps](https://zhuanlan.zhihu.com/p/487809142?)
  * [Displays Operation system information on Raspberry Pi 3B+](https://www.msly.cn/boards/topic/57/installing-home-assistant-core-on-raspberry-pi-3b)
    * [lsb_release -a](https://www.msly.cn/boards/topic/57/installing-home-assistant-core-on-raspberry-pi-3b#1203)
    * [test use domain visit nginx web server](#check-available-versions-for-each-plugin)
    * [Install home assisant core](#create-an-environment)
    * [home assisant core](#activatedeactivate-environment)
      * [https](#activating-in-the-same-shell)
  * [Installing Home Assistant Core on Raspberry Pi 3B+](https://www.msly.cn/boards/topic/57/installing-home-assistant-core-on-raspberry-pi-3b)
    * [Install py](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3701)
    * [test use domain visit nginx web server](#check-available-versions-for-each-plugin)
    * [Install home assisant core](#create-an-environment)
    * [Install nginx](#activatedeactivate-environment)
      * [https](#activating-in-the-same-shell)
  * [Install frp](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3694)
    * [find home assisant core System Info](https://www.msly.cn/boards/topic/3221/bluetooth-speaker-is-silent-checklist#3701)
      * [ find path of configuration.yaml](https://www.home-assistant.io/docs/configuration/)
  * [trouble-Access to HA via chrome browser is not OK](#3698)
      * [1](https://unix.stackexchange.com/questions/258074/error-when-trying-to-connect-to-bluetooth-speaker-org-bluez-error-failed)
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
   
  * [Config](#)
    * [List of Time Zones](https://timezonedb.com/time-zones)  
   

sudo timedatectl set-timezone 'Asia/Shanghai'

ping raspberrypi.local

sqlite3 --version

python3 --version


   docker exec -it ha /bin/sh
/config # hass --version
2025.1.2


## Make Python virtual environment + Home Assistant Core

Install a specific version
~~~
pip3 install homeassistant==2022.5.4
~~~

Restart hass core
~~~
sudo -u homeassistant -H -s
cd /srv/homeassistant
source bin/activate

# run home assistant core with console log
hass -v
~~~

https://www.matterxiaomi.com/boards/topic/57/installing-home-assistant-core-202230-on-raspberry-pi-3b-step-by-step/page/2#2324


Home Assistant Core upgrage
~~~
sudo -u homeassistant -H -s
cd /srv/homeassistant
source bin/activate
pip3 install --upgrade homeassistant
~~~
https://www.matterxiaomi.com/boards/topic/57/installing-home-assistant-core-202230-on-raspberry-pi-3b-step-by-step/page/2#2324




 
