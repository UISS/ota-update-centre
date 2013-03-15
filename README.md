![OTAUpdater Header](http://sensation-devs.org/banner/bannerotaupdate.png)



OTA更新中心
==========

       OTA更新中心是一个更新ROM的应用程序/设备支持通过OTA更新中心.

ROM开发
==========
      你要使用这个软件，去下载部分，下载的最新apk文件。
      这行添加到您的build.prop：
      otaupdater.otaid=（在这里写你的OTA ID没有空格或括号）
      otaupdater.otaver=（在这里写的OTA版本没有空格或括号）
      otaupdater.otatime=（写上日期+时间为：20120820-1516没有空格或括号的）
      如果您的设备有一些奇怪的SD卡（没有/SD卡）命名的OS或recovery，这些行添加到您的build.prop：
      otaupdater.sdcard.os=（SD卡名称（例如sdcard2 /sdcard2）在主系统中不带空格或括号）
      otaupdater.sdcard.recovery=（SD卡名称（例如，sdcard2 /sdcard2）在恢复这里没有空格或括号）
      如果您的设备无法重新启动“adb shell reboot recovery”，写一个脚本，重新启动您的设备，这些行添加到您的build.prop：
      如果你不能写这样一个脚本，使用$$NULL$$去代替路径，接着该应用程序会通过电源管理器尝试重新启动。
          otaudpater.rebootcmd=/path/to/rebootscript.sh -OR- $$NULL$$
      如果自动闪烁该ROM，做一些对您的设备不好的事情，用户需要手动打开手机，添加以下内容到您的build.prop：
          otaupdater.noflash=1
      转到: https://otaupdatecenter.pro 注册一个帐号，并添加/更新你的ROM。

已知的错误
==========
      None so far!


如何建立
==========
      git clone git@github.com:OTAUpdateCenter/ota-update-centre
      
      添加到Eclipse中，进行你的修改，然后导出为一个Android应用程序！:D
