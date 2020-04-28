# Dynamic-motd
Dynamic MOTD for short information when logging in via SSH

~~~
apt-get update && apt-get install figlet lsb-release bc needrestart wget
wget -O /usr/local/bin/dynmotd https://raw.githubusercontent.com/theonlybrand/dynamic-motd/master/dynmotd.sh
chmod +x /usr/local/bin/dynmotd
rm -f /etc/motd
mkdir /usr/local/bin/dynmotd
touch /etc/profile
echo /usr/local/bin/dynmotd >> /etc/profile
touch /etc/zsh/zprofile
echo /usr/local/bin/dynmotd >> /etc/zsh/zprofile
~~~

Upcoming changes
- initial customizing of MOTD
