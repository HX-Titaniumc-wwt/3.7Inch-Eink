# 3.7Inch-Eink
A small but versatile handheld ebook

这是一个3.7英寸的 手持电子书

它带有

·ESP32 WROOM32UE

·MAX98357音频功放

·RX8025T时钟芯片

·SHT30温湿度传感器

·1511扬声器

·1000mAh 3.7Wh的锂电池

·TP4055充电模块

·采用了OKRA 的3.7寸黑白墨水屏作为显示设备

·三个凯华微动按键作为输入设备

·时钟模式下至少能够待机40天

![image](https://github.com/HX-Titaniumc-wwt/3.7Inch-Eink/blob/main/IMG20230620111338.jpg)

制作方法：
1. 从PCB文件夹下载PCB制板文件交给PCB制造商制作（嘉立创可以白嫖），打印外壳
2. 下载BOM表采购零件，注意1uf电容需要耐压25V以上，按键为3*2*3.5侧边按键 + 三枚凯华 “窄”微动
3. 焊接PCB1：以24pin座子为界限，首先焊接座子和type-c之间的零件，焊接完成后测试 typec外壳 和 侧面拨动按键三个引脚 是否短路
4. 焊接PCB2：焊接后续部分电路，并同样测试是否短路（98357功放部分电路如果不使用可以不焊接）
5. 将屏幕插入主板座子，先将屏幕放入壳内屏幕固定框，再进行其他装配

本项目所用到的所有库文件压缩包：
主页面 mhetesp32devkit.7z
下载后解压缩即可

本项目所有自写代码文件压缩包：
主页面 Code.7z
下载后解压缩即可

抱歉，因为我不太熟悉github怎样上传代码，并且直接把工程文件压缩上传超出了25M的限制大小，所以就只能用这种方式来上传代码

To do
