# shell-scripts
Linux Shell Scripts

wget --no-check-certificate https://raw.githubusercontent.com/kuoruan/shell-scripts/master/ovz-bbr/ovz-bbr-installer.sh
chmod +x ovz-bbr-installer.sh
./ovz-bbr-installer.sh

如需卸载，请使用：
./ovz-bbr-installer.sh uninstall

注意：在有firewalld的服务器上安装的时候，firewalld会干扰iptables的规则，造成网络不通（现在具体原因未知，谁有解决方案可以提示一下）。所以在装有firewalld的服务器上需要先退出firewalld：
systemctl stop firewalld
systemctl stop firewalld

