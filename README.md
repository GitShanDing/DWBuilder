# macOS Mojave 动态壁纸生成器 DWBuilder 下载及使用说明
## 下载
支持macOS 14.0的DWBuilder下载地址：https://github.com/Evian-Zhang/DWBuilder/releases/download/v1.1/DWBuilder.dmg

(最后一次更新：2018年10月8日)

## 使用说明
DWBuilder可以生成用户自定义的macOS Mojave支持的动态壁纸。<br>
本程序在设计的时候借鉴了 https://itnext.io/macos-mojave-dynamic-wallpaper-fd26b0698223 的思想，增加了UI，并增加了太阳高度角及太阳方位角的自动计算。<br>

### macOS Mojave 动态壁纸原理
动态壁纸扩展名为.heic, 格式为HEIF格式（High Efficiency Image File Format）,是苹果公司近年来用于存储图片的一种高效图片格式。其编码和解码的工作
已有Nokia相关技术人员完成，可以参看 https://github.com/nokiatech/heif .<br>
每一张系统自带的动态壁纸由16张图片组成，其存储的信息为拍摄该图片时的太阳高度角(elevation)及太阳方位角(azimuth).当用户的Mac所处地点的太阳高度角和太阳方位角
达到对应的角度时，就会自动更换壁纸。这解决了以往动态壁纸无法精确切换白天和黑夜的不足。

### 使用方法
单击"选取..."按钮，依次选取想要合成动态壁纸的图片（经测试，不支持矢量图）。选取成功后，列表中会显示选取图片的名称及URL.<br>
对于每一张列表中的图片，右键单击，选择弹出菜单中的"设置图片信息"，输入拍摄该图片时所处的纬度及时间。（纬度请用小数表示）<br>
单击"导出"，选择相应导出路径，稍等片刻即可生成动态壁纸。

### 软件更新
由于发布动态壁纸后会收到大量用户反馈，苹果公司可能会多次修改动态壁纸的相关方法，如在beta版中有白天模式和黑夜模式等。所以DWBuilder的相关生成方法也会随之改变。因此，在每次macOS的版本更新后，我们都会第一时间更新该软件，请及时检查更新。（在菜单栏中有检查更新一项，会链接到此页面。请查看DWBuilder支持哪些macOS版本)。

### BUG
经测试，会出现预览图与桌面图不一致的情况，疑似桌面图会比预览图提前更换下一张图。这似乎是系统的bug。

### DEMO

我拿了我们东大的李文正图书馆的照片（拍摄+修图：我）和中国传统的天色计时法各做了一个demo，可在 https://github.com/Evian-Zhang/DWBuilder/tree/master/demo 下载。

### 问题反馈

开发者邮箱：evianzhang1999@gmail.com
