# Android
OHA APK
## Android发展历史
1-10
## Android体系结构
五层架构
应用层
应用架构层
依赖库 运行时
硬件抽象层
Linux 内核
## Android的编译
build/envsetup.sh 设置编译环境
Lunch 编译目标
Make 编译整个系统

安卓提供的三种编译
make 整个系统
mmm 指定目录
mm 当前目录
mma 当前目录及其依赖项
## Android的镜像刷机
boot.img 安卓的自定义文件格式
recovery.img 小型文本界面Linux系统
system.img 
app目录 存放一般apk文件
bin目录 一些Linux工具 toolbox的链接
etc目录 系统配置文件
fonts 系统字体文件
framwork目录 系统平台的所有jar包和资源文件包
lib目录 系统库文件
media目录 媒体文件
tts目录 语音文件
xbin目录 谷歌的二进制文件
sbinbuild.prop 系统属性定义文件
user.img 用户数据文件 一般不包含任何文件
## ADB工具的使用
SDK
ADB

## Android设备的GMS认证
一套移动服务应用
GMS应用
CTS测试 系列兼容测试
CTS Verrify 一个手工测试的apk
GTS 谷歌服务测试套件
## Android网站

# Git
git init
git config --global user.name "username"
git config --global user.email "email"
git config --global color.ui true
git config --global core.editor "vim"
git clone
git add .
git commit -m "message"
git rm
git rm -r --cached
git push origin master
git push --tags
git log
git show
git diff

# 手机
## 手机发展史
## 手机通讯知识
WDCMA TD-SCDMA CDMA2000
LTE TD-LTE LTE-A

## 手机研发流程
策划 工业设计 设计与研发 测试与验证 方案整合 设计输出

## 手机构成及其关键器件

# makefile
## 一般格式
target: dependencies
    command

main.o: main.c
    gcc -c main.c -o main.o

## 变量
\$(CC) \$(CFLAGS) \$(INC) \$(LIBS) -o \$(TARGET) \$(OBJS)
### 常用内置变量
\$@ 目标文件
\$< 第一个源文件
\$^ 所有依赖文件

## 伪目标
常见的一些操作
比如clean

.PHONY: clean
clean:
    rm -f \$(OBJS) \$(TARGET)

