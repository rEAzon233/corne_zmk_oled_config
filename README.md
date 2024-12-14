# zmk for keyboards
这是一个存放有多个分体式键盘zmk固件源码以及已编译固件的仓库
corne sofle（RGB，choc） lily58（目前只有这几个，以后或许会有其他键盘放入）
本仓库固件所测试用pcb均来自[PandaKB外设](https://pandakb.taobao.com/shop/view_shop.htm?spm=a21n57.1.0.0.5d79523cNmnkU0&appUid=RAzN8HWMnqHhQPoqPWJj8vvpxQEUo4LsYqKaxNw4JRKQfkmLoFX)
## 仓库中的固件可能有以下功能
### key（基础按键功能）
zmk潜在的comebo，tap dance等按键功能如需要请参照[zmk文档](https://zmk.dev/docs/keymaps)添加代码进行适配
### rgb（zmk光效比较少，四种）
参考[zmk文档](https://zmk.dev/docs/config/underglow)
若需修改灯效，可通过zmk studio添加灯效切换按键
或直接于键盘固件代码config文件中
`CONFIG_ZMK_RGB_UNDERGLOW_EFF_START`
|value|       光效        |
|-|-|
|  0  |       纯色        |
|-|-|
|  1  |       呼吸        |
|-|-|
|  2  |       光谱        |
|-|-|
|  3  |       旋流        |
### zmk studio（zmk studio是zmk推出的在线改键软件，包括app及web，其中web支持usb改键，app同时支持usb改键以及蓝牙改键）
usb改键[zmk studio_web在线改键](https://zmk.studio/)
app改键[zmk studio_app](https://github.com/zmkfirmware/zmk-studio/releases/tag/v0.2.4)

usb改键只需连接分体键盘左手即可进行改键，蓝牙改键只需键盘处于连接状态打开app进行匹配就可进行改键
（注：zmk studio的启用暂处于起步阶段，功能支持有限，相比于已较为完善的via以及vial改键，仍有发展空间，zmk studio目前支持功能请参考[zmk文档](https://zmk.dev/docs/features/studio)
### 键盘休眠
没什么好说的，请参考[zmk文档](https://zmk.dev/docs/config/power#low-power-states)
电池上报√ rgb休眠√ 休眠时间设置√ 
### oled
默认的oled显示的内容用了github上开源的zmk module[nice_oled](https://github.com/mctechnology17/zmk-nice-oled?tab=readme-ov-file)
这个module是动画的，还是很好玩的，同时感谢作者的开源@mctechnology17
![image](https://github.com/mctechnology17/zmk-nice-oled/blob/main/assets/preview2.JPG?raw=true)
