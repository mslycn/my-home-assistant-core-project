
接近**大金（Daikin）、三菱电机（Mitsubishi Electric）、松下（Panasonic）**等日系空调的「舒眠模式（Sleep Mode）」

## 建立体感温度概念 apparent temperature

| 温度  | 湿度  | 体感    |
| --- | --- | ----- |
| 30℃ | 40% | 28.8℃ |
| 30℃ | 60% | 30.4℃ |
| 30℃ | 80% | 32.0℃ |



不要只根据温度控制，而是根据体感温度 + 湿度 + 时间三者共同控制

| 因素   | 是否需要  | 说明            | 空调            | 直到           |
| ---- | ----- | ------------- |------------- |-- |
| 第一阶段（刚睡）   | 人体散热最高，快速把人体热量带走  | If 温度 >30℃ Humidity >70%   | Cooling 26℃ Fan High  | 温度下降到28℃  |
| 第二阶段（熟睡））   | 人体代谢下降  |     |Cooling 27℃ Fan Low  | 不要一直26℃。 否则容易半夜冷醒  |
| 第三阶段（凌晨）   | 凌晨3点以后人体最低体温  |    | Cooling 28℃ Fan Low  | 室温<27℃  Fan Only  |
| 第四阶段（快起床）   | 人体散热最高  |    | 室温>29℃  则Cooling 27℃ | 避免热醒  |


主要遵循下面几个原则：
~~~
入睡30分钟快速降温
熟睡后慢慢升高设定温度
凌晨避免人体失温
优先降低湿度，而不是一味降低温度
风速越来越小
避免压缩机频繁启停
~~~


configuration.yaml

~~~
climate:
  - platform: broadlink
    name: Vaillant AC
    host: IP address of the Broadlink device
    mac: 'MAC address of the Broadlink device'
    ircodes_ini: 'broadlinkcodes/vaillant.ini' #path of the .ini file
    min_temp: 18
    max_temp: 25
    target_temp: 23
    target_temp_step: 1
    temp_sensor: sensor.your_temperature_sensor #entity_id of your temperature sensors
    default_operation: idle
    default_fan_mode: low
    customize:
      operations:
        - idle
        - cool
      fan_modes:
        - low
        - mid
        - high

~~~

see:https://github.com/mario-g0/HA-climate-vaillant/blob/master/configuration.yaml
