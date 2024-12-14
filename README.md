rgb√
oled√
zmk studio√

（1.去除“CONFIG_ZMK_RGB_UNDERGLOW_EXT_POWER=y”，修复关闭rgb灯同时关闭oled屏幕的bug


2.限制rgb最大亮度为60（支持最大亮度为100）


3.增加蓝牙上报电池电量


4.修复corne.dtsi文件内行列错误


5.设置rgb初始灯效）2024.11.11


(添加nice view的配置：
lily58：√
todo：corne sofle）

（todo：nice view玩法教程）
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
`CONFIG_ZMK_RGB_UNDERGLOW_EFF_START`的值进行修改
|value|       光效        |
|  0  |       纯色        |
|  1  |       呼吸        |
|  2  |       光谱        |
|  3  |       旋流        |
