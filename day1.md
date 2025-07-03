# adb命令
开发和调试 Android 应用时更高效地操作设备
## 设备管理
adb devices
adb connect 192.168.1.100:5555
adb disconnect

## 应用安装与卸载
adb install app-debug.apk
adb innstall -r app-debug.apk
adb uninstall com.example.app
adb shell pm clear com.example.app

## 日志查看
adb logcat
adb logcat -v time
adb logcat *:W
adb bugreport

## 文件操作
adb push file1 /sdcard/file1
adb pull /sdcard/file1 file1
adb shell ls /sdcard
adb shell rm /sdcard/file1
adb shell mkdir /sdcard/mydir

## Shell操作
adb shell
adb shell am start -n com.example.app/.MainActivity
adb shell pm list packages
adb shell input keyevent 4
adb shell screenshot -p /sdcard/screenshot.png
adb shell sccreenrecord /sdcard/screenrecord.mp4
## 其他命令
adb reboot
adb reboot bootloader
adb reboot recovery
adb root
adb remount

## 与应用交互
adb shell start -r com.example.app/.MainActivity
adb shell startservice -a android.intent.action.VIEW -d http://www.baidu.com
adb shell am broadcast -a android.intent.action.VIEW -d http://www.baidu.com
adb shell am force-stop com.example.app

## 查看设备信息
adb shell getprop ro.product.model
adb shell dumpsys battery
adb shell wm size
adb shell wm density
adb shell dumpsys window display
adb shell settings get secure android_id
adb shell dumpsys iphonesubinfo
adb shell service call iphonesubinfo 1
adb shell getprop ro.build.version.release
adb shell cat /proc/meminfo
adb shell ifconfig
adb shell cat /proc/cpuinfo

# BAT脚本
按顺序执行一批命令
REM ::
ECHO
PAUSE
FIND
IF
EXIT
COPY
DATE
DEL
TYPE
< >
:>>
|
可以和adb命令结合使用

# Linux命令
usermod -s /bin/bash root
which a
su -
exit
chowm a b
chgrp a b
chmod 777 a

date
cal
df -h
du -h

ps aux
top
kill -9 1234

find a -name "*.txt"
ln -s
ln

tar -cvf a.tar /file
tar -xvf a.tar /file
tar -zcvf a.tar.gz /file
tar -zxvf a.tar.gz -C /file
tar -jcvf a.tar.bz2 /file
tar -jxvf a.tar.bz2 -C /file

ls -l -a -h
cd 
touch
rm
mkdir
pwd
tree
cp
mv
 cat
 more
 grep
 echo a > a.txt
 shutdown
 ifconfig
 ping ip
 scp -P port
 Ctrl + C
 ssh -p port user@ip
 chmod 777
 groupadd
 cat /etc/passwd
 chgrep -R

 useradd -m -g
 userdel -r
 passwd

 cat /etc/group
 id
 usermod -g
 usermod -G

 # vi editor
 三种模式：1. 命令模式 2. 输入模式 3. 搜索模式
 