
<p align="center">
  <strong>
    <a href="">website</a>
    •
    <a href="">docs</a>
    •
    <a href="">community</a>
    •
    <a href="">add-ons</a>
  </strong>
</p>

# home-assistant  core  project

# Beginners guide to use smart devicesgit with HomeAssistant

从零开始搭建一套HomeAssistant智能家居系统

A Complete Smart Home Solution.It is possible to install Home Assistant Core without Docker. However, it is a more complex process that requires advanced technical knowledge. Users need to install Python, set up a virtual environment, and install Home Assistant Core manually. A step-by-step guide can be found on this doc.

To learn the Home Assistant system from the beginning, it is best to install manually, from a virtualenv!

Home Assistant系统搭建详细教程

树莓派安装操作系统
树莓派安装Home Assistant

Home Assistant配置详细教程


Home assistant integration设备接入详细教程

Home Assistant远程管理详细教程


### 本项目对应于《HomeAssistant智能家居实战篇》系列内容中的文档。
[home-assisant.msly.cn](https://home-assisant.msly.cn)

## Contents
* [Install homeassistant core](#install-homeassistant-core)
* [Install Node red for home assistant core](#install-node-red)  
* [Install Homebridge](#install-homebridge)  
* [Install MatterBridge for home assistant core](#install-matterbridge)
* [Install ESPHome for home assistant core](#install-esphome)

* [Home Assistant Remote access](#Home-Assistant-Remote-access)

## Install homeassistant core

1. [home assisant project-install home assisant core 2022.3.0 on Raspberry Pi3b+](https://github.com/mslycn/home-assistant/blob/main/home-assisant-core-install.MD)
	- [硬件环境准备——安装树莓派]
    - [软件环境环境准备——树莓派操作系统](https://www.matterxiaomi.com/boards/topic/57/installing-home-assistant-core-202230-on-raspberry-pi-3b-step-by-step/page/3#18932)  - Raspberry Pi system information and version   Raspberry Pi OS 是基于 Debian 的免费操作系统，针对 Raspberry Pi 硬件进行了优化.
	- [系统环境设置——树莓派基础配置](https://www.matterxiaomi.com/raspberry-pi-3)  - Raspberry Pi hardware version
	- [Install Raspberry Pi OS on a Raspberry PI SD-card 树莓派安装 Raspberry Pi OS 系统](https://www.msly.cn/boards/topic/2184/install-raspberry-pi-os-on-a-raspberry-pi-sd-card) - 首先，树莓派需要安装 Raspberry Pi OS 系统，教程:烧录 镜像 到sd卡
	- [How to Upgrade Raspberry Pi OS to the Latest Version? (Debian 12,Bookworm)](https://www.matterxiaomi.com/how-to-upgrade-raspberry-pi-os-to-the-latest-version-2022) -升级 Raspberry Pi OS 系统教程:
	- [基于树莓派安装HomeAssistant core](https://github.com/freemsly/home-assistant/blob/main/home-assisant-core-install.MD)
	- [HomeAssistant配置、文件结构、升级]
	  - [Home Assistant Core upgrage](https://www.msly.cn/boards/topic/57/installing-home-assistant-core-on-raspberry-pi-3b/page/2#3590)
      - [HomeAssistant自启动如何配置]
	- [HomeAssistant core 20221102配置、文件结构、升级]
	  - [http://192.168.2.50:38123/profile](http://192.168.2.50:38123/profile)
	  - [change Home Assistnant Core default port](https://www.msly.cn/boards/topic/13395/quick-start#18747)
      - [Home Assistnant Core Initial configuration](https://www.matterxiaomi.com/boards/topic/13395/quick-start#18951) - Home Assistnant Core
	Initial configuration , First configuration

1. [Install Home Assistant Docker On Windows Using VMware Workstation 17 Pro series)](https://blog.matterxiaomi.com/blog/windows10-vmware-home-assistant-docker-part1/)


1. [Install Home Assistant OS On Windows Using VMware Workstation 17 Pro series)](https://blog.matterxiaomi.com/blog/install-home-assistant-os-on-windows10-vmware-pro-part1/)
   - [home assistant on your windows 10 machine using wsl( ubuntu for windows)]

1. [host - Proxmox VE]
   - [Install Proxmox VE via ISO image](https://pve.proxmox.com/pve-docs/chapter-pve-installation.html)
   - [Install Proxmox VE on Debian](https://pve.proxmox.com/pve-docs/chapter-pve-installation.html#_install_proxmox_ve_on_debian)



## ssh client

2. [ssh client]
	- [xshell]() you access HA directly via (xshell and xftp)SSH port 22 on windows 10
	- [Enable SSH on Raspberry Pi](https://blog.matterxiaomi.com/blog/raspberry-pi-ssh-server-part1/) Enable SSH on Raspberry Pi raspberry pi os lite (64-bit)
	- [Other]
	  - [How to Install Home Assistant core 2022.3.0 on Ubuntu 20.04（vultr VPS） Step by Step ](https://www.iaspnetcore.com/Blog/BlogPost/624b26f5bc7b674a02f93b86/how-to-install-home-assistant-core-202230-on-ubuntu-2004vultr-vps-step-by-step) - no pve + vultr VPS
	  - [How to install full Home Assistant Core in Python virtual environment on Debian 11 operating system(x86_64 with python virtual environment) Step by Step](https://www.matterxiaomi.com/how-to-install-full-home-assistant-core-on-debian-11-operating-systemwith-python-virtual-environment-step-by-step)  - pve + vultr VPS
      - [install Home Assistant core on debian Server](https://blog.matterxiaomi.com/blog/install-home-assistant-core-debian-server/)  - pve + vultr VPS
      - [How to Get the correct Debian ISO](https://www.matterxiaomi.com/boards/topic/36/debian-11-bullseye-installation#63)
	  - [树莓派3B安装home assistant全过程](https://www.cnblogs.com/mokou/p/14423917.html)
	  - [Raspberry Pi 5中文文档](https://pidoc.cn/docs/computers/raspberry-pi-5)


3. Docker
	- [Learn to install Docker properly on Raspberry Pi OS](https://itsfoss.com/raspberry-pi-install-docker/) 
	- [Learn to How To Install Docker and Docker-Compose On Raspberry Pi properly](https://www.dotruby.com/articles/how-to-install-docker-and-docker-compose-on-raspberry-pi#4-install-docker-compose)     

	- [File Editor - Samba server]() File Editor  just install Samba on the host machine that points to your docker files. If your config files for Home Assistant are located in /srv/docker/homeassistant, for example, then  setup a Samba server and setup a share in the /srv/docker/homeassistant,Then you can just edit from there with your normal text editor on any machine.  on Windows you use \\<IP_ADDRESS>\
	- [File Editor - hass-configurator-docker](https://github.com/CausticLab/hass-configurator-docker) Linux x32/64 and ARM builds for the hass-configurator.  
	- [File Editor - hass-configurator](https://github.com/danielperna84/hass-configurator) 
	- [File Editor - VSCode server](https://www.linuxserver.io/our-images?name=linuxserver/code-server)  OPEN WEB UI to open Studio Code Server.

Learn to install Docker properly on Raspberry Pi OS in this tutorial.	

3. 组件接入基础篇
	- [让设备发声——朗读文字 小度音箱]         edge tts
	- [让设备发声——朗读文字 小爱player]
	- [让设备发声——朗读文字 小爱pro老版]      edge tts
	- [让设备发声——朗读文字 小米音箱pro新版]
	- [让设备发声——朗读文字 PC]
	- [让设备发声——朗读文字 android phome]
	- 让设备看到——使用手机摄像头做监控
	- 接入硬件产品——小米多功能网关
	- 接入自定义组件-和风天气
	- [接入Logitech media server](#)
	- [Plex Media Server]
	- [Spotify Connect]
4. 操作进阶篇   
    - 设置地理位置与界面语言
	- 实体显示属性自定义
	- [系统信息 - System Health integration](https://www.home-assistant.io/integrations/system_health) - System Health integration data can be viewed at Settings -> System -> Repairs -> System Information in the overflow menu (top right).
	- [配置目录](http://192.168.2.50:8123/config/repairs) - Configuration Directory	/home/homeassistant20221103/.homeassistant

6. 设备位置追踪篇
	- 设备定位准备知识与Ping检测
	- nmap网络扫描、黑客、小米wifi路由器
	- [home assisant project-Play audio on a Bluetooth speaker with Raspberry Pi3b+](https://github.com/freemsly/home-assistant/blob/main/home-assisant-bluetooth-speaker.MD)
	- 使用iCloud随时定位苹果手机
7. 自动化篇
	- [python_scripts中文](https://blog.51cto.com/u_16213299/11996185) 在Home Assistant 中运行 Python 代码
	- [python_scripts](https://blog.51cto.com/u_16213299/11996185)  <config>/pyscript folder

	- [<config>/pyscript](https://hacs-pyscript.readthedocs.io/en/stable/tutorial.html#writing-your-first-script) 官方例子里，pyscript可以用来代替jinja，可以代替yaml写出自动化和script。生成的service可以直接被调用
	- [pyscript 安装教程](https://hacs-pyscript.readthedocs.io/en/stable/installation.html)  安装好后从integration中添加即可,手动安装请见https://hacs-pyscript.readthedocs.io/en/stable/installation.html
	- [pyscript使用教程](https://bbs.hassbian.com/thread-16211-1-1.html)
	- 语音+音乐+灯光闹钟
7. 自动化篇
	- [automation 示例代码](https://github.com/Petro31/home-assistant-config/blob/dc0827ed770f0dc2fa37d66191543e8021ee8769/scripts/zwave_js.yaml#L130) 在Home Assistant 中运行 automation 示例代码	


7. HomeAssistant创建模板实体(Template) 通过代码模拟出各种各样的智能家居设备
	- [基于状态的模板(template)传感器、二元传感器、按钮、数字项和选择项](https://bbs.hassbian.com/thread-18160-1-1.html)
	- [Template integration](https://www.home-assistant.io/integrations/template/)
	- [HomeAssistant创建模板实体(Template)-light,开关](https://www.cnblogs.com/Luad/p/18606120)
	- 预留
	- 预留
	- 预留
7. 设备接入篇 Light
	- [通断器]()   不支持凌动，不支持调节亮度和色温；
	- [凌动通断器]()   不支持调光
	- [3C凌动通断器]()  不安全
	- [单色温调光驱动]        调色温
	- [双色温调光驱动]        调色温
	- [三色温调光驱动]        调色温
	- [电源驱动]
	- 预留	

8. 设备接入篇(1)
	- 太阳、月亮、季节和潮汐
	- 天气与预报——yr、DarkSky、……
	- 红外遥控——博联RM系列产品
	- 红外遥控——小米万能遥控器
	- 文件夹监测——FolderWatche
	- 云端的自动化——IFTTT(2)
	- 系统性能监控——SystemMonitor
8. PC接入篇
	- [HASS.Agent](https://github.com/mslycn/HASS.Agent) c#
	- PC RTSP协议摄像头与ffmpeg
	- PC ONVIF协议摄像头
	- PC 麦克风
	- PC 音箱
	- PC 自动开机

8. Player Providers - DLNA
    - [Android手机DLNA]   Android手机：全功能DLNA：安装MirageDLNA
	- [PC DLNA Media Renderer](http://localhost:4999/boards/topic/21966) 	Kodi DLNA Media Renderer on pc.Windows Media Player ,Install VLC Media Player,Install Kodi

8. 各种摄像头接入篇
	- 支持MJPEG的摄像头与图片抓取
	- RTSP协议摄像头与ffmpeg
	- ONVIF协议摄像头
	- 有线树莓派CSI与USB摄像头
	- 小米的大方摄像头
	- 天气预报与交通状况图——另类摄像头
9. 本地AI摄像头-人脸识别篇
    - [Reolink RLC-810A AI camera with local Person & Vehicle detection](http://localhost:4999/boards/topic/48305/reolink-rlc-810a-ai-camera-with-local-person-vehicle-detection)  connect Reolink RLC-810A AI camera to home assistant
	- DLib配置与pip安装
	- 本地DLib人脸探测
	- 本地DLib人脸识别
	- 微软人脸特征检测
	- 微软人脸识别与验证
	- Facebox-在docker中运行人脸识别
9. 本地离线语音篇 stt
	- [whisper中文语音识别服务（CPU版本]
	- [xinnan-techxiaozhi-esp32-server](https://github.com/xinnan-tech/xiaozhi-esp32-server/pull/96/files) 增加支持home assistant语音助手,home assistant api访问令牌  https://github.com/xinnan-tech/xiaozhi-esp32-server/pull/96/files

	- [docker wyoming-vosk](https://blog.matterxiaomi.com/blog/docker-vosk-1/) how to build a standalone container for vosk using the wyoming protocol. 
	- [Docker wyoming-vosk for Home Assistant]()  github.com/mslycn
	- [rhasspy/wyoming-speech-to-phrase](https://github.com/OHF-Voice/speech-to-phrase)	 Speech-to-phrase is targeted at lower-end hardware.
    - [yaming116/sherpa-onnx-asr]
	- [yaming116/fun-asr]
	- 预留	
9. 本地离线语音篇 stt projects that use Vosk
	- [docker wyoming-vosk](https://blog.matterxiaomi.com/blog/docker-vosk-1/)  A standalone container for vosk using the wyoming protocol. for home assistant docker
	- 预留		

	
22. DIY智能音箱
	- DIY智能音箱（1）——整体架构、硬件安装
	- DIY智能音箱（2）——snowboy、speech_recognition
	- DIY智能音箱（3）——完成主程序架构
	- DIY智能音箱（4）——与HomeAssistant交互
	- [Rhasspy Voice Assistant](https://rhasspy.readthedocs.io/en/latest/) it works with Hermes protocol compatible services (Snips.AI) Home Assistant and Hass.Openhub
	- [Wyoming Satellite](https://github.com/rhasspy/wyoming-satellite) Wyoming Satellite 是一个使用 Wyoming 协议的远程语音项目，通过ESP32或类似硬件实现本地唤醒词检测和stt功能
	- [Wyoming Satellite 远程语音卫星源码工作原理](https://mmssai.com/archives/4386) 远程语音智能音箱，使用Wyoming协议，进行本地唤醒词检测和音频增强，接入智能家居系统ha
	- [基于esphome的语音助手]
	- [Assist Microphone]() uses a local USB microphone to control Voice Assist.
	- [Atom Echo语音助手教程](https://sumju.net/?p=9542#google_vignette)  Atom Echo语音助手 接入ha教程。
9. 本地离线语音篇 AI
	- [Home Assistant 接入 ChatGPT](https://tonnie17.github.io/posts/home-assistant-chatgpt/)
	- 预留	
9. 本地离线语音篇 mcp
	- [mcp server and mcp client](https://www.cnblogs.com/edisonchou/p/-/introduction-to-mcp-csharp-sdk)  此时与ha无关，分为客户端和服务端
	- 预留			

10. Brand ZigBee网关设备接入篇（2）
	- [Aqara Gateway 集成子设备接入 HA](https://community.aqara.com/pc/#/post/postDetail/1045)
	- [Aqara Bridge integration](https://github.com/bernard3378/AqaraBridge)  Aqara Bridge - 用官方云API把Aqara设备接入HA
	- Wi-Fi 设备（例如 Aqara 的妙控开关S1E、人在FP2  设备接入 HA 里的 HomeKit 控制器
	- [Integrating Philips Hue Bridge with Home Assistant](https://pimylifeup.com/home-assistant-philips-hue/)  Philips Hue Bridge
	- [Ikea]
	- [tuya]
	- [terncy hub](https://github.com/rxwen/homeassistant-terncy-component)  吧网关接入ha https://github.com/rxwen/homeassistant-terncy-component

11. 开源Zigbee hub接入篇(Diy Zigbee network)
    - [connect-zbt1 zha](https://neiltw.com/home-assistant-connect-zbt1-setup-guide/#google_vignette)	Best way to add Zigbee and Matter to Home Assistant.
	- [connect-zbt1 z2m](https://blog.csdn.net/feilusia/article/details/145135102)
	- [connect-zbt1 Zigbee2MQTT](https://neiltw.com/how-to-use-zigbee2mqtt-to-intergrate-zigbee-devices-in-home-assistant)	
	- [SONOFF Zigbee 3.0 USB Dongle Plus Gateway]()  use a Sonoff Zigbee stick for mine and it works well and is as plug and play as anything. where to buy? https://www.amazon.com/SONOFF-Gateway-Universal-Assistant-Wireless/dp/B09KXTCMSC
	- [SONOFF Zigbee 3.0 USB Dongle Plus V2]
	- [Home Assistant 基于EZSP Zigbee Dongle创建Zigbee智能家居系统](https://www.smartlabs.cn/home-assistant-%e5%9f%ba%e4%ba%8eezsp-zigbee-dongle%e5%88%9b%e5%bb%bazigbee%e6%99%ba%e8%83%bd%e5%ae%b6%e5%b1%85%e7%b3%bb%e7%bb%9f/)  zigbee zha
9. aqara设备接入篇(2)    
	- [aqara hub M1s](https://www.msly.cn/boards/topic/5278/aqara-gatewayhub-g2h-m1s-cn-p3-cn-m2-cn-h1-cn-e1-cn-g3-cn-g2h-pro-integration-for-home-assistant#18735)
	
10. Aqara hub M2组件接入基础篇(IOS users)
	- [1.Paired aqara m2 to Homekit(IOS users)](https://blog.matterxiaomi.com/blog/Add-aqara-m2-to-Homekit/)
	- 让设备看到——使用手机摄像头做监控
	- 将消息发送给你的邮箱
	- 接入硬件产品——小米多功能网关
	- [接入自定义组件-和风天气]()
	- [小米中枢网关接入Home Assistant Core专业实战教程（mi home app + Xiaomi Miot Auto Integration）](https://zhuanlan.zhihu.com/p/552370350)
	- 将消息发送给你的邮箱
	- 接入硬件产品——小米多功能网关
	- 接入自定义组件-和风天气 
	
11. 使用苹果设备语音控制篇
	- 通过Homekit与苹果Siri连接(1)
	- 通过Homekit与苹果Siri连接(2)
	- 捷径与HA的接口调用
	- 在HA中完成语音文字处理——chrome语音控制
	- 苹果设备语音控制全自由定制
	- [esp-homekit-devices](https://github.com/RavenSystem/esp-homekit-devices)
	- [c# Homekit.Net](https://www.cnblogs.com/hezp/p/18142099) 通过c#代码模拟出各种各样的智能家居设备，并添加到苹果手机的家庭app中
11. 手机接入篇 消息通知  短信 消息到手机 ha app
	- [中移ML307R模块]() 购买链接：https://item.taobao.com/item.htm?ft=t&id=795927858234
	- [GSM-modem Integration]()  you can explore the SMS notification via GSM-modem integration in Home Assistant to directly send messages to your Home Assistant instance
	- [List of USB GSM stick modem or device](https://www.home-assistant.io/integrations/sms/#required-hardware) USB GSM stick modem or device like SIM800L v2 connected via USB UART.
	- 将消息发送给你的邮箱     send an email
	- 将消息发送给你的手机
	- 通过Homekit与苹果Siri连接(2)
	- 捷径与HA的接口调用
	- 苹果设备语音控制全自由定制
	- [把android手机变成dlna音箱]	  安装airpin u apk
12. Midea 接入篇

12. haier 接入篇
 
12. 数据记录篇
	- 历史数据基础概念
	- 数据组件的配置、mysql数据库及其它
13. AppDaemon与DashBoard
	- 安装、配置与初步运行
	- DashBoard配置(1)
	- DashBoard配置(2)
	- 制作App——一个最简单的样例
	- 制作App——应用callback
	- [Picture elements card 2D](https://thehomeautomationblog.com/how-to-create-a-floorplan-in-home-assistant-part-5-interactive/) How to create a floorplan in home assistant
	- [Picture elements card 2D](https://pacossmarthome.co.uk/control-your-house-in-home-assistant-with-a-picture-elements-card/) Control your house in Home Assistant with a Picture Elements Card
	- [Custom Mushroom card](https://bbs.hassbian.com/thread-21857-1-1.html)  代码使用案例
	- [Auto-entities]

## Install Node red
14. Installing Node red for Home Assistant Core
	- [Install node-red](https://www.matterxiaomi.com/boards/topic/14538/node-red-node-red) - Installing Node red for Home Assistant Core 2023.2.2 in a Python vEnv on Raspberry Pi 3B+ step by step
	- Node-RED配置
	- HomeAssistant节点(1)
	- [https://nodered.org/docs/getting-started/docker](https://nodered.org/docs/getting-started/docker) install configure and run node-red in docker
	- [https://github.com/node-red/node-red](https://github.com/node-red/node-red)
## Install Homebridge Integration
14. Installing Homebridge for Apple Home app  

    - [使用 Homebridge Docker 将米家设备接入 Homekit](https://juejin.cn/post/7265630149322997794?searchId=2025021100330020E901919E863C4359F0)
	- [Install Homebridge](https://blog.matterxiaomi.com/blog/install-uninstall-reinstall-homebridge-raspbian-part1/) - Installing Homebridge for 
	- [涂鸦远程红外遥控器 + Home Assistant 接入苹果家庭(homekit)](https://zhuanlan.zhihu.com/p/1920988695982486609)
	Apple Home app
	- Node-RED配置
	- HomeAssistant节点(1)
	- HomeAssistant节点(2)
	- 一些样例：闹钟、自动湿度控制、门铃
## Install  matter server Integration
14. Installing matter server for for Home Assistant Core
	- BLE
	- [Connect ZBT-1 Thread border router](https://www.home-assistant.io/integrations/thread/#turning-home-assistant-into-a-thread-border-router)  how to use Connect ZBT-1 to turn your Home Assistant into a Thread Border router.Turning Home Assistant into a Thread border router.
	- MatterBridge
	- matter binding
	- List of compatible Matter Devices
	- Matter Bridge  Add-on
	- [树莓派配置mDNS服务 Avahi](http://localhost:4999/boards/topic/21933/%E4%B8%BA%E6%A0%91%E8%8E%93%E6%B4%BE%E9%85%8D%E7%BD%AEmdns%E6%9C%8D%E5%8A%A1-avahi)  http://localhost:4999/boards/topic/21933/%E4%B8%BA%E6%A0%91%E8%8E%93%E6%B4%BE%E9%85%8D%E7%BD%AEmdns%E6%9C%8D%E5%8A%A1-avahi
	- [Part 1 - Matter Server in Home Assistant](https://blog.matterxiaomi.com/blog/Matter-Home-Assistant-part1/)
	- [Part 5 - Install Matter Server using docker image via docker run](https://blog.matterxiaomi.com/blog/matter-home-assistant-part5/)
    - [matter设备配网流程工作原理图文解释 ](http://www.chinasem.cn/article/349653)  三种配对方式流程介绍
	- [matter设备配网流程工作原理 三个阶段 ](https://blog.csdn.net/m0_46411607/article/details/131564958)
	- [matter设备配网流程工作原理 源码级别 ](https://www.cnblogs.com/youhui/p/18715676)

## Install  OTBR Integration
14. Installing Open Thread Border Router for for Home Assistant Core
	- [options OTBR devices for Home Assistant Core](https://community.home-assistant.io/t/choosing-the-right-thread-radio-thread-border-router/824676?u=msly) - 
	- [Notes on implementing Matter](https://community.home-assistant.io/t/notes-on-implementing-matter/423484)
	- [SkyConnect - silabs multiprotocol and docker](https://community.home-assistant.io/t/skyconnect-silabs-multiprotocol-and-docker/526779)  This solution takes an HA OTBR AddOn and modifies it to run as a stand-alone Docker container
	- [SLZB-06](https://smlight.tech/manual/slzb-06/guide/thread-matter/)
	- [SONOFF Dongle-E]
	- [a Stable Matter over Thread Network](https://www.derekseaman.com/2024/09/essential-tips-for-a-stable-matter-over-thread-network.html)
	- [https://openthread.google.cn/guides/border-router/build?hl=zh-cn](https://openthread.google.cn/guides/border-router/build?hl=zh-cn)  penThread 边界路由器构建和配置
	- [Make Apple TV 4K (3rd Gen) as a Thread Border Router in Home Assistant as the preferred network](https://community.home-assistant.io/t/apple-tv-as-thread-border-router-not-adding-to-preferred-network/847644) 
	- [Build border router thread 1.4 firmware for ESP32-H2](https://www.matteralpha.com/how-to/how-to-build-a-thread-1-4-border-router)  via Espressif SDK


## Install  MatterBridge Integration
14. Installing MatterBridge for for Home Assistant Core
	- [Install  MatterBridge](https://blog.matterxiaomi.com/blog/matter-bridge-part1/) - Installing MatterBridge for for Home Assistant Core
	- [https://github.com/Luligu/matterbridge](https://github.com/Luligu/matterbridge)
	- [https://github.com/t0bst4r/home-assistant-matter-hub](https://github.com/t0bst4r/home-assistant-matter-hub)  This project simulates bridges to publish your entities from Home Assistant to any Matter-compatible controller like Alexa, Apple Home or Google Home.
15. 树莓派GPIO口设备连接篇
	- 直连树莓派的LED(1)——NodeRED接入/HA中rpi_gpio_pwm组件
	- 直连树莓派的LED(2)——HA 中的shell_command/binary_sensor.command_line/light.template
	- 直连树莓派的温湿度传感器
16. MQTT Integration篇
	- [服务器安装EMQX](https://blog.csdn.net/weixin_43808708/article/details/145711960)
    - [MQTT服务器接入Home Assistant和.NET程序](https://blog.csdn.net/farway000/article/details/142548023) 搭建EMQX MQTT服务器并接入Home Assistant和.NET程序
	- QoS、retain、last_will、自动配置……


18. 成为HomeAssistant开发者
	- 组件的工作原理
	- [integration template](https://github.com/ludeeus/integration_blueprint) a template for HA integrations. a "blueprint" that custom integration blueprint developers 
	- [https://github.com/krahabb/meross_lan](https://github.com/krahabb/meross_lan) a realwore sample that use https://github.com/ludeeus/integration_blueprint
	- [DIY集成](https://blog.iin0.cn/blogs/skill/node/ha-to-koishi.html#koishi%E6%8E%A5%E5%85%A5ha)  blog
	- [DIY集成开发-脚手架脚本-ZhongshengConfig设备](https://blog.csdn.net/Cubar/article/details/143158313) python3 -m script.scaffold inetgration vscode 方式开发，包含自动发现
	- [基于 STM32 和米家WiFi模块 ESP8266 的智能插座的设计与实现](https://blog.csdn.net/qq_40431685/article/details/140263631)	IOT开发  基于 STM32 和 ESP8266 的智能插座的设计与实现
19. IOS App的使用
    - [https://github.com/home-assistant/iOS](https://github.com/home-assistant/iOS) IOS apk 下载
	- IOS App——连接、定位与通知消息
	- iBeacon定位
	- 多媒体通知与静态文件Web服务
19. Home Assistant Companion App的使用
    - [https://github.com/home-assistant/android](https://github.com/home-assistant/android) android apk 下载  Dowanload mobile app  on your Android or iPhone
    - [https://github.com/home-assistant/iOS](https://github.com/home-assistant/iOS) IOS apk 下载
	- [nesror大佬的ha app](https://github.com/nesror/Home-Assistant-Companion-for-Android) github的nesror大佬的ha app，非常好用，推荐指数五颗星。Github（Android+iOS）
	- iBeacon定位
	- 多媒体通知与静态文件Web服务
20. Lovelace定制界面
	- 理解Lovelace页面的结构
	- Lovelace中的卡片
	- 使用自定义lovelace卡片
21. 抓取Internet信息作为传感器
	- 即时股票行情——使用sensor.rest
	- 各种网站页面元素——sensor.scrape组件
23. 音乐灯带
	- 音乐灯带——硬件连接与基本使用
	- Arduino与ESP硬件
	- 音乐灯带——音频处理过程与Arduino平台编译
	- [雷特驱动查询网址](https://www.ltech.cn/html/Products/)
24. 远程麦克风
	- [声音信号的采集与播放-Arduino IDE](https://blog.csdn.net/m0_74276051/article/details/143181595) 如何使用ESP32开发板与INMP441麦克风模块进行音频采集，并通过UDP将音频数据传输到Windows主机进行播放。
	- [声音信号的采集与播放-Arduino IDE](https://www.180it.com/archives/2151/) 使用ESP32开发板与INMP441麦克风模块进行音频采集，c# 服务端接收代码
	- [声音信号的采集与播放-Arduino IDE](https://lingshunlab.com/book/esp32/esp32-using-inmp441-microphone-module-for-real-time-audio-data-acquisition) 使用ESP32开发板与INMP441麦克风模块进行音频采集，c++ 代码
	- 接入HomeAssistant的远程麦克风
	- 使用远程麦克风——监听与录音
	- 给智能音箱配上远程麦克风
	- [ESP32-S3-Box3-Custom-ESPHome](https://github.com/BigBobbas/ESP32-S3-Box3-Custom-ESPHome)  This firmware will enable your S3 Box 3 to use the touch screen and home button, and configure the box to act like a dashboard for Home Assistant. Giving you the power to control your entitities and display sensor information.The box will also be configured as a media player, giving you volume control (also improves the overall volume of the internal speaker compared to the ESPHome stock config) and easily broadcast messages to the device or stream media. Oh, and don't forget! it is also a Voice Assistant!!
    - [ESP32-S3-BOX-3 部署 Home Assistant 本地化語音助理教程](https://neiltw.com/esp32-s3-box-3-ha-local-voice-assistant-guide/)
	- [ESP32-S3-BOX-3 部署 Home Assistant 本地化語音助理教程2](https://neiltw.com/en/esp32-s3-box-3-ha-local-voice-assistant-guide/)  修改支持的语言
	- [如何给Home Assistant添加一个ESP32-S3-BOX-3开源硬件语音助手设备](https://blog.csdn.net/Slaven230101/article/details/145813994)   csdn
	- [How to Run Wyoming Satellite and OpenWakeWord on Android](https://community.home-assistant.io/t/how-to-run-wyoming-satellite-and-openwakeword-on-android/777571/52)
	
25. 485总线
	- 实现485总线通讯
	- 接入自定义ascii码指令集的设备
	- 接入modbus设备
	- 自定义二进制命令设备的接入
26. KNX
	- 家庭总线部署方案与KNX
	- 使用IPRouter接入HomeAssistant
	- 使用ncn5120模块-USB连接模式
	- 使用ncn5120模块-WIFI连接模式
27. 室外物联网
	- 全球卫星定位
	- [GPS定位Traccar使用教程]
	- NB-IOT
	- 车载定位(1)—traccar安装与配置
	- 车载定位(2)—车载设备diy
	- [Gpslogger app]
	- [Owntracks app]
28. docker
	- [docker home assistant基础(1)](https://github.com/home-assistant/core/releases)   https://github.com/home-assistant/core/releases
	- [Home Assistant Base Images](https://github.com/home-assistant/docker-base)   Debian	bookworm, trixie
	- [Home Assistant Base Images](https://github.com/home-assistant/docker-base)   The Debian	bookworm, trixie image include S6-Overlay, Bashio and TempIO.
	- HomeAssistant的docker安装
	- HomeAssistant docker容器的典型使用
	- HomeAssistant docker容器的非典型使用
28. DIY红外与433转发设备 ir
	- 使用红外与无线模块(1)——红外接收
	- 使用红外与无线模块(2)——红外发射
	- 使用红外与无线模块(3)——无线收发
	- 硬件制作(1)——画电路图
	- 硬件制作(2)——画PCB板
	- 硬件制作(3)——元器件与焊接
	- [博联设备 via Broadlink Integration](https://www.cnblogs.com/softlin/p/16511684.html)	
	- [Broadlink RM4 Pro -Remote: Learn command](https://www.bazmac.me/blog/using-broadlink-rm4-pro-with-home-assistant)	Broadlink RM4 Pro guide: 
28. API
	- RHTTP API     API服务提供商都会有一个使用政策，规定如何合法地使用他们的API服务。用户需要遵守这些政策，注册账户，并获取API密钥
	- RESTful API 
	- Websocket API 实现服务器与客户端之间的实时双向通信，可以用来推送最新信息到用户界面.
## Home Assistant Remote access
29. Home Assistant Remote access - frp
	- [buy a domain from www.namesilo.com ](https://www.iaspnetcore.com/Blog/BlogPost/5eb9e65e775d020216dbe009/wwwnamesilo-operation-manual-for-com-registration-and-domain-name-purchase)
	- [buy a vps server from vultr]()
	- [A to server]()
	- [install nginx on Raspberry Pi](https://www.iaspnetcore.com/Blog/BlogPost/5d9865cc72c1772b244afe0f/how-to-install-and-uninstall-reinstall-nginx-on-ubuntu-1804aliyun)
	- [config nginx for your domain](https://www.iaspnetcore.com/Blog/BlogPost/579b2ab584cd462440deb4f4/how-to-configure-aspnet-core-to-work-with-reverse-proxy-serversnginx)
	- [install Let’s Encrypt client certbot]()
	- [Opne Firewall port 80 and 443 on vultr]()
	- [Install on  Frp Client on Raspberry Pi ](https://www.matterxiaomi.com/boards/topic/30/how-to-install-frp-on-home-assistant-operating-systemhassos-on-raspberry-pi-step-by-step)
	- [CloudFlare](https://www.iaspnetcore.com/Blog/BlogPost/5ee3a43a1c73d43127f113a1/cloudflare-free-cdn-website-acceleration-practice-tutorial#mcetoc_1g37gn9lf11)
	- Basic Firewall Setup
	- [downloaded SSL certificates for your domain](https://www.iaspnetcore.com/blogpost-6449555969967f028d52f122-how-to-install-and-uninstall-reinstall-mysql-on-ubuntu-1804vultr)
	- [synology nas 安装 docker frpc](https://rainwu.cn/archives/synology-frp-openvpn)	
	
5. [home assisant project-remote access on Raspberry Pi3b+](https://github.com/freemsly/home-assistant/blob/main/home-assisant-remote.MD)
	- 申请Amazon免费云主机
	- [buy a domain from www.namesilo.com](https://www.iaspnetcore.com/Blog/BlogPost/5eb9e65e775d020216dbe009/wwwnamesilocom-registration-and-domain-name-purchase-operation-manual)
	- frp隧道构建
	- 免费为HA配上域名与HTTPS网站证书
	- nginx代理
	- [Install Let’s Encrypt Client Certbot](https://www.iaspnetcore.com/blogpost-619a0dbd5b26cb0202ae5bf1-how-to-secure-nginx-with-lets-encrypt-on-ubuntu-1804vultr#mcetoc_1g3p82cte53) - 666
	- [Let’s Encrypt Client certbot验证域名所有权](https://www.iaspnetcore.com/Blog/BlogPost/5c2874c21d51ae0eec5ece63/the-type-verification-and-certbot-client-type-of-free-certificate-for-total-station-deployment-https-4-lets-encrypt)	- 本文描述用standalone 方式： certbot 自己运行一个 web server 来进行验证域名所有权后生成证书		
    
- Home Assistant Remote access - The Possible Solutions
	- [Securing Home Assistant with Cloudflare Zero Trust](https://empty.coffee/home-assistant-cloudflare-zero-trust-setup/)  Cloudflare Add-on
	- []
	- [Tailscale]( ) WireGuard-based
	- [Python虚拟环境]
- 加餐
	- 使用TensorFlow进行物体识别
	- 使用NFC识别不同的ID卡
	- ESPHome中的自动化
	- 制作树莓派镜像文件(1)
	- 制作树莓派镜像文件(2)
28. Multi-Room Music Solution works with home assistant 实现音乐服务器
   
_I was able to cook up a fun audio setup controlled and automated with Home Assistant! It features
Multiple room synchronised audio speakers (fixed/analog, portable Bluetooth devices and via app on phone or tablet)
Playback of internet radio, Spotify streaming and local audio files.
Sound notifications for Doorbell, garden gate and other sensors and home alarm events.

Install Plex, Jellyfin, Kodi, or Universal Media Server.Many different media servers support DLNA.

Options for Multi-Room Music Solution

Snapcast 是一个开源的多房间音频同步播放系统._

专业音频：与AirPlay/Spotify Connect

    - [Mopidy Server]()  a music server that can play local files, or connect to streaming music services like Spotify.
	- [Logitech Media Server](https://community.home-assistant.io/t/how-to-build-a-lms-based-whole-house-audio-system/436016)  Logitech Media Server服务器,通过安装插件，LMS可以将局域网内支持airplay、Chromecast、DLNA等协议的设备进行统一管理，统一控制；
	- [synchronous multiroom audio with Snapcast]  Snapcast 是一个开源的多房间音频同步播放系统,.服务器端：需安装 snapserver 客户端：需安装 snapclient
	- [Snapcast Server]() which enables synchronized audio streaming across your network.  Snapcast is a multi-room client-server audio player, where all clients are time synchronized with the server to play perfectly synced audio. Snapcast Client是一个接收并同步播放来自Snapcast Server音频流的客户端程序，支持多平台和设备，允许构建低延迟同步的多房间音频系统It's not a standalone player, but an extension that turns your existing audio player into a Sonos-like multi-room solution.
	- [Plex Media Server]() 树莓派Raspberry Pi 安装Plex Media Server并挂载USB硬盘打造微型家庭影音服务器
	- [Music Assistant Server](https://www.michaelsleen.com/music-assistant/)  How to Setup Music Assistant in Home Assistant 
	- [Music Assistant Server-Add Player Provider](https://alshowto.com/add-multi-room-to-home-assistant/)  Add Player Provider(squeezelite)
	- [Spotify Connect] Spotify Connect is a feature that allows you to stream music from Spotify to compatible devices (like speakers, TVs, or gaming consoles) over Wi-Fi or a local network, using your phone, tablet, or computer as a remote control. 
	- [picoreplayer](https://www.picoreplayer.org/)
**Recommended hardware for multi room audio**
 
    - [Set Up Windows 10 as DLNA Renderer]   Intall Kodi,vlc as DLNA Renderer
28. 影音系统	实现影音服务器
	- [树莓派 Raspberry Pi 安装 Kodi 影音系统](https://zhuanlan.zhihu.com/p/364985735)   安装LibreElec系统
28. 镜像投屏 Mirror Iphone to TV

一般投屏的协议通道，三种。
   DLNA最常用，爱奇艺优酷腾讯哔哩哔哩等视频投屏都是用DLNA投屏协议。
   MIRACAST协议，这个主要用于镜像，比较少用。
   Airplay协议苹果手机的屏幕镜像功能，视频APP里的airplay入口都是airplay投屏协议，
   最后是lelink协议
    
	- [RPiPlay 项目](https://github.com/FD-/RPiPlay) RPiPlay项目暂只适合播放PPT,卡得要死
	- [balena-rpiplay 项目](https://sspai.com/post/70302)  balena-rpiplay 可以把你的树莓派变成 Airplay Server，用户把苹果设备的屏幕镜像串流到树莓派上，而树莓派则通过 HDMI 连接电视/显示器/投影仪，部署了这个项目以后算是 Apple TV 盒子中 Airplay 功能的平替。
	- [Shairport-sync]( https://github.com/mikebrady/shairport-sync) broadcast an audio stream from your phone to the main device. The broadcast will be via Airplay
	- [How to Setup a Raspberry Pi as an AirPlay Receiver](https://fleetstack.io/blog/raspberry-pi-airplay-receiver) 使用树莓派安装shairport-sync使老音响变身AirPlay音响	
	- [iPhone镜像投屏到电视](https://www.apeaksoft.com/zh-CN/mirror-screen/mirror-iphone-to-tv/)	 如何将 iPhone 镜像到 Apple TV;将 iPhone 镜像到支持AirPlay电视

- 直播源
	- [一个国内可直连的直播源分享项目](https://github.com/fanmingming/live) - 一个国内可直连的直播源分享项目
	- [https://github.com/topics/tv](https://github.com/topics/tv) - https://github.com/topics/tv
	- [树莓派DIY电视盒子Libreelec](https://blog.csdn.net/saga1979/article/details/109570366) 树莓派DIY电视盒子,安装Libreelec + 小米蓝牙遥控器
	- [Libreelec in ProxMox]()   Quick guide to running Libreelec in ProxMox
	
	- HA实时直播画面(by Bobo)
28. NAS - Synology
    - [Installing Home Assistant docker on a Synology  NAS](https://philhawthorne.com/installing-home-assistant-io-on-a-synology-diskstation-nas/)
	- [How to Use Home Assistant as an NAS Server](https://umatechnology.org/how-to-use-home-assistant-as-an-nas-server/)
28. NAS - 飞牛fnos
	- [飞牛OS部署docker mqtt](https://post.smzdm.com/p/al8w60pp/)	群晖或者飞牛OS部署docker mqtt
    - [飞牛NAS 虚拟机 安装Home Assistant OS(HAOS)](https://www.xiaoxu.vip/archives/218.html)
28. NAS - TrueNAS 
	- [安装TrueNAS服务器–第1部分](https://blog.csdn.net/shengbro1989/article/details/140666451)	虚拟机64bit安装TrueNAS ISO（网络附加存储）教程 –第1部分
    - [如何在TrueNAS中配置ZFS存储和NFS共享 - 第2部分](https://blog.csdn.net/shengbro1989/article/details/140952943?spm=1001.2101.3001.10752)
	- [TrueNAS：使用Plex Media Server创建自己的“家庭媒体流服务器” - 第3部分](https://blog.csdn.net/shengbro1989/article/details/141127938)


## Install ESPHome Integration
17. DIY智能硬件ESP32篇
    - [开始使用ESPHome：如何安装和集成它与家庭助理?](https://www.21ic.com/a/977576.html)
    - [Installing and configuring ESPHome with ESP8266 and ESP32](https://chelmiki.com/posts/installing-and-configuring-esphome/)
	- [ESP32-引脚图（ESP-WROOM-32](https://blog.csdn.net/lianyinghhh/article/details/139971338)
	- [ESP8266——固件烧录与连接-Windows10识别到32硬件](https://blog.matterxiaomi.com/blog/esphome-esp32-part1/#mcetoc_1ide17tct1)
	- ESP8266上的MicroPython使用
	- 连接ESP8266的DHT温湿度传感器
	- ESP8266完成各种功能
	- 典型样例讲解：光照传感器与智能灯
	- [搭建个人智能家居 3 -第一个设备“点灯”](https://blog.csdn.net/qq_42250136/article/details/136673356)
	- ESPHome——不编程，集成ESP8266
	- 音乐灯带——接入ESPHome(1)
	- [ESPHome 继电器控制](https://blog.csdn.net/yueyeguzhuo/article/details/118060420)
    - [Installing mirror lighting on ESPHome](https://chochol.io/en/smart-home/home-assistant-installing-mirror-lighting-on-esphome/)
	- [ESP32 SIM800L](https://randomnerdtutorials.com/esp32-sim800l-send-text-messages-sms/) ESP32 SIM800L: Send Text Messages (SMS Alert) with Sensor Readings
	- [esphome制作零火智能开关](https://blog.csdn.net/zuobianfy/article/details/118432775) esphome制作零火智能开关,esp01s继电器一个
	- [Touch Screen Controller](https://esphome.io/components/touchscreen/tt21100.html) Touch Scr	

	- [使用XIAO ESP32C6 Zigbee 连接继电器控制HomeAssistant中的单色LED条](https://www.21ic.com/a/983542.html)	XIAO ESP32C6 Zigbee固件 接入 HomeAssistant connect ZBT-1
18. 成为ESPHome开发者
	- [POE Bluetooth Proxy and ESPHome](https://smlight.tech/manual/slzb-06/guide/bluetooth-proxy/)  SLZB-06x utilize ESP32 chip so can be used as a ESPHome Bluetooth proxy adapter for Home Assistant
	- [用ESPHome烧录固件到合宙ESP32-C3并接入HomeAssistant](https://blog.csdn.net/sinat_15906013/article/details/147806199)  SLZB-06x utilize ESP32 chip so can be used as a ESPHome Bluetooth proxy adapter for Home Assistant


- 精彩众创教程
	- 魔镜系列——魔镜安装(by JonnyWong)
	- 魔镜系列：天气组件openweather(by JonnyWong)
	- 魔镜系列：第三方组件WeeklySchedule(by JonnyWong)
	- 魔镜系列：获取HomeAssistant中实体状态(by JonnyWong)
	- 魔镜系列：联动智能音箱(by JonnyWong)
	- 在群晖中安装ESPHome(by Bobo)
	- ESPHome-SonoffBasic完整接入过程(by Bobo)
	- ESPHome-接入SonoffRF(by Bobo)
	- ESPHome-接入SonoffPow(by Bobo)
	- ESPHome-接入Sonoff4CH4路继电器(by Bobo)
	- ESPHome-H801玩转RGB+冷暖光(by Bobo)
	- Esphome-空气质量传感器(by Bobo)
	- EspHome-DIY小屏幕(by Bobo)
	- 设计与制作PCB板(by Zack-Xu)
	- 树莓派安装HASS.IO(by Zack-Xu)
	- HASSIO.IO与常规运行环境区别(by Zack-Xu)
	- x86下ubuntu虚机及HomeAssistant安装（by 猛将兄）
	- [dfrobot sensor](https://wiki.dfrobot.com/HUSKYLENS_V1.0_SKU_SEN0305_SEN0336)  diy sensor via dfrobot brand
	
4. matterxiaomi
	- [create vps on vultr](https://www.iaspnetcore.com/Blog/BlogPost/6199ff495b26cb0202ad6ce8/how-to-deploy-a-new-instance-on-vultr-step-by-step)
	- [Install xshell7 on windows 10](https://www.iaspnetcore.com/Blog/blogpost/635d3024da4aea5b6ab5891e)
	- [How to Install and uninstall reinstall  upgrade .NET on Ubuntu 18.04 64](https://www.iaspnetcore.com/Blog/BlogPost/618a75d3635c733c81dc77c3/how-to-install-and-uninstall-reinstall-upgrade-net-6x-on-ubuntu-180464-step-by-step)
	- [How to Deploying Real World ASP.NET Core  on Ubuntu 18.04 step by step(client <-> backend web server)](https://www.iaspnetcore.com/Blog/BlogPost/5d9833c672c1772b244aa228/how-to-deploying-real-world-aspnet-core-3x-on-ubuntu-1804-step-by-step)
	- [how to Configure ASP.NET Core to work with Reverse Proxy servers(client <-> proxy(nginx) <-> backend web server)](https://www.iaspnetcore.com/Blog/BlogPost/579b2ab584cd462440deb4f4/how-to-configure-aspnet-core-to-work-with-reverse-proxy-serversnginx)
	- [How To Install and uninstall reinstall Nginx on Ubuntu 18.04（aliyun/vultr）](https://www.iaspnetcore.com/Blog/BlogPost/5d9865cc72c1772b244afe0f/how-to-install-and-uninstall-reinstall-nginx-on-ubuntu-1804aliyun)
	- [Firewall Setup on vultr](https://www.iaspnetcore.com/Blog/BlogPost/6199ff495b26cb0202ad6ce8/how-to-deploy-a-new-instance-on-vultr-step-by-step#mcetoc_1g2gdbgp550)
	- [www.namesilo.com域名购买教程](https://xmmblog.com/namesilo-domain-registration/)
	- [www.namesilo.com域名购买教程](https://blog.csdn.net/dafei5210/article/details/115410981)
	- [www.namesilo.com](https://www.iaspnetcore.com/Blog/BlogPost/5eb9e65e775d020216dbe009wwnamesilo-operation-manual-for-com-registration-and-domain-name-purchase)
	- [CloudFlare](https://www.iaspnetcore.com/Blog/BlogPost/5ee3a43a1c73d43127f113a1/cloudflare-free-cdn-website-acceleration-practice-tutorial#mcetoc_1g37gn9lf11)
	- Basic Firewall Setup
	- [How To Install and uninstall reinstall Mysql on Ubuntu 18.04（vultr）](https://www.iaspnetcore.com/blogpost-6449555969967f028d52f122-how-to-install-and-uninstall-reinstall-mysql-on-ubuntu-1804vultr)	
		
4. CloudFlare
	- [CloudFlare 免费CDN网站加速实战教程之1：注册、DNS 解析记录](https://www.iaspnetcore.com/Blog/BlogPost/5ee3a43a1c73d43127f113a1/cloudflare-free-cdn-website-acceleration-practical-tutorial-1-registration-dns-resolution-records)
	- [Install xshell7 on windows 10]()
	- [How to Install and uninstall reinstall  upgrade .NET on Ubuntu 18.04 64]()
	- [How to Deploying Real World ASP.NET Core  on Ubuntu 18.04 step by step(client <-> backend web server)](https://www.iaspnetcore.com/Blog/BlogPost/5d9833c672c1772b244aa228/how-to-deploying-real-world-aspnet-core-3x-on-ubuntu-1804-step-by-step)
	- [how to Configure ASP.NET Core to work with Reverse Proxy servers(client <-> proxy(nginx) <-> backend web server)](https://www.iaspnetcore.com/Blog/BlogPost/579b2ab584cd462440deb4f4/how-to-configure-aspnet-core-to-work-with-reverse-proxy-serversnginx)
	- [How To Install and uninstall reinstall Nginx on Ubuntu 18.04（aliyun/vultr）](https://www.iaspnetcore.com/Blog/BlogPost/5d9865cc72c1772b244afe0f/how-to-install-and-uninstall-reinstall-nginx-on-ubuntu-1804aliyun)
	- [Firewall Setup on vultr](https://www.iaspnetcore.com/Blog/BlogPost/6199ff495b26cb0202ad6ce8/how-to-deploy-a-new-instance-on-vultr-step-by-step#mcetoc_1g2gdbgp550)
	- [www.namesilo.com](https://www.iaspnetcore.com/Blog/BlogPost/5eb9e65e775d020216dbe009/wwwnamesilo-operation-manual-for-com-registration-and-domain-name-purchase)
	- [CloudFlare](https://www.iaspnetcore.com/Blog/BlogPost/5ee3a43a1c73d43127f113a1/cloudflare-free-cdn-website-acceleration-practice-tutorial#mcetoc_1g37gn9lf11)
	- Basic Firewall Setup
	- [How To Install and uninstall reinstall Mysql on Ubuntu 18.04（vultr）](https://www.iaspnetcore.com/blogpost-6449555969967f028d52f122-how-to-install-and-uninstall-reinstall-mysql-on-ubuntu-1804vultr)	

- Home assistant training course
    - Home assistant online course for developers	

## 树莓派
   - [亚博 树莓派 非官方代理](https://www.yahboom.com/study/4wd-Pi)  taobao:树莓派精品销售商 https://shop101688001.taobao.com/ 
   - [上海上海晶珩 8G/4G](https://edatec.cn/zh/sbc/Pi5?src=raspberrypi)  taobao:树莓派特卖店 https://2etuqghaurnjs9utgnob2rkzr1rc15a.taobao.com/
                                               

 - [全屋wifi history](https://mp.weixin.qq.com/s?__biz=MzkwNDMyNjE1OQ==&mid=2247487843&idx=1&sn=b96486858569c4ffb4bcb5f554f2f7ff&chksm=c089ec03f7fe6515cf331a95c05083125c7277fcc86f5a6023fc73466e30e4cd9c92e4275073#rd)	
 - [各品牌路由器、组网结构](https://github.com/blanboom/awesome-home-networking-cn/blob/master/README.md?plain=1)
		
## Useful links
1. 全屋智能的HA配置 真实案例 share configuration<br>
My heartfelt thanks to:

https://github.com/sl041400/Home-assistant

https://github.com/matt8707/hass-config

https://github.com/relliky/Tais_Home_Assistant_Config

https://github.com/Snipercaine/DrZzs-HA

https://github.com/Snipercaine/home_assistant_config

2. 小米有品<br>
https://www.xiaomiyoupin.com/

2. 小米商城
https://www.mi.com/index.html

https://linptech.tmall.com/

https://linptech.jd.com/

https://opple.tmall.com/


3. awesome-ha<br>
[https://www.awesome-ha.com](https://www.awesome-ha.com/)

4. yeelight forum<br>
[yeelight forum](https://forum.yeelight.com/latest)

5. bbs<br>
https://www.mydigit.cn/thread-475884-1-1.html

https://www.right.com.cn/

https://bbs.eeworld.com.cn/

https://www.chiphell.com/

https://ngabbs.com/

https://www.chinadsl.net/

6. blog<br>
https://post.smzdm.com/

https://blog.iin0.cn/

7. web<br>
https://neiltw.com/

8. project
https://oshwhub.com/

立创商城
https://www.szlcsc.com/

三色灯带

https://item.szlcsc.com/546079.html

9. web search
https://www.aipan.me/

10. web ai search

https://chat.deepseek.com/

https://yuanbao.tencent.com/

10. Only for china user

- Home Assistant OS 极速版

https://www.hasscn.top/about.html

- HassBox

https://hassbox.cn/


- 冬瓜HAOS

http://hasshome.net/

https://www.wghaos.com/


