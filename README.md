# boot_tools
Brush recovery for virtual a/b partition devices.
请确保手机为vab分区机型，以root方式执行脚本
使用前请使用rec解包工具对要刷入的rec进行解包
并将解包出的ramdisk放入./rec_install_tool/ramdisk文件夹

<刷入ramdisk.sh>自动刷入vab机型的rec
<备份boot.sh>自动备份原镜像
<恢复boot.sh>自动恢复原镜像

rec解包教程:
将要刷入rec复制或移动到本目录并命名为recovery.img
执行<解包rec.sh>
解包出的ramdisk就在本目录

OTA系统更新说明：
第一次请使用完整包更新
系统更新更新前执行<恢复boot.sh>(第一次不用)
到系统更新页面下载OTA更新包更新
系统更新校验完成后
先执行<备份boot.sh>后执行<刷入ramdisk.sh>
在Magisk中使用安装到未使用的槽位来刷Magisk
重启后就会有第三方rec和Magisk
