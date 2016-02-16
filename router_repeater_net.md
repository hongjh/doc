##路由器设置 无线中继增大wifi覆盖
家庭路由器覆盖面积有限，从路由利用WDS无线分布系统(从路由需要wds 主路由不需要)，对信号中继，扩大覆盖面。本质是从路由WDS连上主路由（从路由无需网线），然后提供wifi服务。

###主路由开启无线功能
一般来说，已经在使用的无线路由器设置不需要修改。从路由像其它手机终端或pc终端能连上主无线路由就可以了。
1. 无线工作模式：AP无线接入点。（正常就是这个工作模式）
2. 设置信道，主从路由一致。这里选择 频道11
3. DHCP可以由此主路由提供，可以开启。

###从路由设置WDS
因为叫中继，所以ssid使用和主路由一致的 wifi名称，其实使用不同的名称也是可以的。
1. 设置和主路由一致的ssid和密码
2. 选择和主路由一致的信道
3. 开始WDS. （这个是关键，这样从路由工作是可以无需网线，配置的时候还是需要的）
4. 填写主路由的ssid和bssid; 也可以使用扫描，选择，这样比较方便  
填写正确的密码，保证能连上主路由
5. 关闭从路由的DHCP，这个可以交给主路由处理
6. 设置LAN：比如主路由是192.168.0.1;从路由可以设置为192.168.0.2
7. 从路由WAN不需要设置，不需要
