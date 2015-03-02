# vpn_tunnel_service
A systemd service for maintaining SSH tunnel when using VPN

# File list
/etc/sysconfig/sshtunnel
/usr/lib/systemd/system/sshtunnel.service
/usr/lib/systemd/user/sshtunnel.service

# Use a soft link
Use a soft link for /usr/lib/systemd/user/*
ln -s /usr/lib/systemd/system/sshtunnel.service /usr/lib/systemd/user/sshtunnel.service

# Remote host
The default remote host name is remotesystem, either create a host entry for this or edit /etc/sysconfig/sshtunnel
