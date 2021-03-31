This binaries correspond to the following

```
NodeMCU 3.0.0.0
        branch: evmik-WeMos-master_20191216
        commit: a64af6cbc4cd53a376ab6cb0597dbaf921de9c81
        release: 1.4.0-master_20151229 +1129
        release DTS: 201912161819
        SSL: false
        build type: float
        LFS: 0x0
        modules: adc,bit,dht,file,gpio\item 2c,mqtt,net,node,ow,rtctime,spi,tmr,uart,u8g2,wifi
 build 2019-12-16 15:00 powered by Lua 5.1.4 on SDK 3.0.1-dev(fce080e)
```

To flash run

```
~/src/cloned/esptool/esptool.py --port /dev/ttyUSB0 write_flash 0x00000 ./0x00000.bin 0x10000 ./0x10000.bin 0x3fc000 ./esp_init_data_default.bin -fm dio -fs 32m
```

