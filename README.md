# DalamudCNAdapter
为国际服Dalamud启用中文字体支持方案
[toc]
## 前言

​	国际服游戏默认不包含中文字库，且Dalamud的国际服分发字体默认不包含中文一些字体，导致主界面与部分插件在一些中文状态下缺失，显示为===，目前有两种方法为国际服Dalamud启用中文字体支持下面我会介绍这两种方法的过程与利弊。（个人推荐方法2）

## 方法1  为游戏补全中文中文字库

​	使用Dalamud中的Penumbra插件为游戏热加载中文字库，字库可以在https://github.com/AinaSnow/DalamudCNAdapter/raw/master/resources/ChnFontRange.ttmp2 下载导入到Penmubra后勾选启用，在Dalamud设置里启用AXIS字体即可。
![](https://s2.loli.net/2023/08/28/37rXPyexOkvAJKj.png)

### 优点

游戏内字体得到了补充且稳定，但dalamud依旧缺少字体 只是一些有dalamud发出的在聊天框内的提示文字得到了补全
![](https://s2.loli.net/2023/08/28/5OblxqkGEXS3zaM.png)

### 缺点

dalamud本身的字体未得到补充依旧是===基本属于没什么用，插件内字体依旧![1.png](https://s2.loli.net/2023/08/28/uEOwPB6THYf4QIA.png)

## 方法2 使用相关的Dalmaud插件

​	使用https://github.com/AinaSnow/DalamudCNAdapter 该项目中的插件来为Dalamud本身替换字体来补全缺失的中文部分，右侧releases下载[DalamudCNAdapter.zip](https://github.com/AinaSnow/DalamudCNAdapter/releases/download/1.0.0.0/DalamudCNAdapter.zip)，下载完后解压缩放到自己想放到的位置，复制DalamudFontReplacer.dll的路径填写到Dalamud设置的开发板路径中，保存并启用设置自启动即可。
![7.png](https://s2.loli.net/2023/08/28/qxjzLEfkltMsTF7.png)

### 优点

​	直接补全了Dalamud自己的字体 使得UI内/插件内的中文完美显示无错误，精简了CJK中的韩文减少字体大小提高稳定性
![5.png](https://s2.loli.net/2023/08/28/SfvYHlsqXtAMkan.png)

### 缺点

​	稳定性较差，启动的时候有5%的概率直接炸游戏需要二次启动，且在主界面的时候无法使用右侧的悬浮栏 会99.5%炸游戏，登陆后使用/xldev交互没任何问题，游戏内dalamud发送到聊天窗口的文字依旧受游戏本身影响。
![6.png](https://s2.loli.net/2023/08/28/3PfFnHy1UJRdGBk.png)
