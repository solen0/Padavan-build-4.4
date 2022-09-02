- RM2100_4.4.3.9-100.trx

  ```yml
  ##科学上网##
  echo "CONFIG_FIRMWARE_INCLUDE_SHADOWSOCKS=n" >> .config #科学上网插件，选择n后全部有关插件都不集成
  echo "CONFIG_FIRMWARE_INCLUDE_XRAY=n" >> .config #集成xray执行文件 ~4.5M
  echo "CONFIG_FIRMWARE_INCLUDE_V2RAY=n" >> .config #集成v2ray执行文件
  echo "CONFIG_FIRMWARE_INCLUDE_TROJAN=n" >> .config #集成trojan执行文件 ~0.5M
  echo "CONFIG_FIRMWARE_INCLUDE_SSOBFS=n" >> .config #simple-obfs混淆插件
  ##科学上网##
  
  ##DNS服务##
  echo "CONFIG_FIRMWARE_INCLUDE_SMARTDNS=n" >> .config #smartdns
  echo "CONFIG_FIRMWARE_INCLUDE_ADGUARDHOME=n" >> .config #adg DNS去AD
  
  ##内网穿透服务##
  echo "CONFIG_FIRMWARE_INCLUDE_ZEROTIER=y" >> .config #zerotier ~1.3M
  echo "CONFIG_FIRMWARE_INCLUDE_ALIDDNS=y" >> .config #aliddns
  echo "CONFIG_FIRMWARE_INCLUDE_DDNSTO=y" >> .config #ddnsto ~0.5M
  echo "CONFIG_FIRMWARE_INCLUDE_WIREGUARD=y" >> .config #wireguard ~10k
  
  echo "CONFIG_FIRMWARE_INCLUDE_FRPC=y" >> .config #内网穿透FRPC
  echo "CONFIG_FIRMWARE_INCLUDE_FRPS=y" >> .config #内网穿透FRPS
  echo "CONFIG_FIRMWARE_INCLUDE_TUNSAFE=y" >> .config #TUNSAFE
  ##内网穿透服务##
  
  echo "CONFIG_FIRMWARE_INCLUDE_MENTOHUST=y" >> .config #mentohust
  
  echo "CONFIG_FIRMWARE_INCLUDE_CADDY=y" >> .config #在线文件管理服务
  echo "CONFIG_FIRMWARE_INCLUDE_ALDRIVER=y" >> .config  #ALDRIVER  ~3m
  ```

- K2P_4.4.3.9-100.trx

~~~yml
##科学上网##
echo "CONFIG_FIRMWARE_INCLUDE_SHADOWSOCKS=y" >> .config #科学上网插件，选择n后全部有关插件都不集成
echo "CONFIG_FIRMWARE_INCLUDE_XRAY=y" >> .config #集成xray执行文件 ~4.5M
echo "CONFIG_FIRMWARE_INCLUDE_V2RAY=y" >> .config #集成v2ray执行文件
echo "CONFIG_FIRMWARE_INCLUDE_TROJAN=y" >> .config #集成trojan执行文件 ~0.5M
echo "CONFIG_FIRMWARE_INCLUDE_SSOBFS=y" >> .config #simple-obfs混淆插件
##科学上网##

##广告管理##
echo "CONFIG_FIRMWARE_INCLUDE_ADBYBY=n" >> .config #adbyby plus+
##DNS服务##
echo "CONFIG_FIRMWARE_INCLUDE_SMARTDNS=n" >> .config #smartdns
echo "CONFIG_FIRMWARE_INCLUDE_ADGUARDHOME=n" >> .config #adg DNS去AD


##内网穿透服务##
echo "CONFIG_FIRMWARE_INCLUDE_ZEROTIER=n" >> .config #zerotier ~1.3M
echo "CONFIG_FIRMWARE_INCLUDE_ALIDDNS=n" >> .config #aliddns
echo "CONFIG_FIRMWARE_INCLUDE_DDNSTO=y" >> .config #ddnsto ~0.5M
echo "CONFIG_FIRMWARE_INCLUDE_WIREGUARD=n" >> .config #wireguard ~10k
##内网穿透服务##
echo "CONFIG_FIRMWARE_INCLUDE_ALDRIVER=n" >> .config  #ALDRIVER  ~3m
echo "CONFIG_FIRMWARE_INCLUDE_MENTOHUST=n" >> .config #mentohust

##流控QOS##
echo "CONFIG_FIRMWARE_INCLUDE_SQM=y" >> .config #SQM QOS#CPU超频
echo "CONFIG_FIRMWARE_INCLUDE_OC=n" >> .config #CPU超频开关
echo 'CONFIG_FIRMWARE_MT7621_OC="0x312"' >> .config #此处填写对应频率的十六进制：1000Mhz=0x312 1100Mhz=0x362 1120Mhz=0x372 1200Mhz=0x3B2
echo "CONFIG_FIRMWARE_INCLUDE_ALDRIVER=y" >> .config  #阿里云盘  ~3m
~~~

