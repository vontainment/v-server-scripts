# proxmox-host2vm-tty

Set Proxmox host ttyX to connect to VM serial port

Move vm-terminal-tty2.service to /etc/systemd/system

systemctl stop getty@tty2.service
systemctl disable getty@tty2.service
systemctl mask getty@tty2.service

systemctl enable vm-terminal-tty2.service
systemctl start vm-terminal-tty2.service