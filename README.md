# Hackintosh-High-Sierra-10600KF-GTX1070-MSI-Z490i-Unify
90% completed hackintosh build with 10th Gen Intel cpu and 1070 (pretty uncommen combination)  
这一奇幻搭配是一个怪异时代（矿潮）的产物，由于老机子（8600k）主板报废，直接购买了10代新平台板U而显卡暂时不准备更换了（事实证明购买带核显的cpu会是更好的选择），不过除了无法开启显卡硬解，其他都还好。

测试支持 Support tested : High Sierra 10.13.6(17G14042)
 
#### 配置/Hardware info
| 规格     | 详细信息                                                                       |
| -------- | ------------------------------------------------------------------------------ |
| 型号     |                                                                                |
| 主板     | 微星 MEG Z490I UNIFY                                                          |
| 处理器   | 英特尔 Core i7-10600KF @ 4.10GHz 六核                                           |
| 内存     | 16 GB ( Gskill DDR4 3000MHz )                                                  |
| 硬盘     | Intel 760p                                |
| 显卡     | GTX 1070 ( 8 GB / 技嘉itx )                                        |
| 无线网卡 | 英特尔® Wi-Fi 6 AX201 ( 板载 )                                                 |
| 声卡     | 板载                                                                           |
| 触摸板   |                                                                                |
| 触摸屏   |                                                                                |


#### BIOS
1.Secure Boot                [Disabled]  
2.Disk set to AHCI  
3.XMP                        [Enabled]  
4.CFG Lock                   [Disabled]  
5.SGX                        [Disabled]  

#### 使用/Issues
 **使用说明:** 
 1. 有线网卡：
    表现为网络中以太网显示电缆被拔出，无信号。
	需要 高级--硬件--设置速度和双工，
		速度：根据你的路由器来，如果是百兆的口，就选100，千兆的选1000。
		双工：选节能以太网，如果还是不行，换其它的。
 		如果还不能解决，尝试手动设置固定ip和dns
    
 2. 无线网卡：
    你可能需要将AirportItlwm.kext添加到S/L/E并关闭SIP才能正常使用

 3. 未解决unsolved：
    无核显硬解：查找大量资料并尝试开启但没有成功，似乎需要免驱独显才能开启
    睡眠：睡眠问题似乎是这块主板的通病，请等待微星官方给出解决方法，目前关闭睡眠使用
