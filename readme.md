# got dex
360加固，乐固等软件的脱壳程序
Android studio 3.6可直接运行
## 软件说明

通过hook 得到脱壳后的dex

* 需要基于xposed 框架

## 使用步骤
* 安装xposed框架（可通过模拟器安装）
* clone本项目，编译apk
* 安装apk，激活模块
* 启动got dex，设置要脱壳的应用包名，确定重启
* 启动要脱壳app，稍等片刻后，查看对应目录`/data/data/{packageName}/ `下是否有dump出来的dex
* `adb pull   /data/data/{packageName}/  电脑目录`
* 尽情撸dex