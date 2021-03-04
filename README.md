# dnsexit
Dynamic DNS updating via DNSExit

Many thanks to jhonnymonclair for his repo!

This repo only contains a minor fix for updating just <em>one</em> A record:
```host2.example.com```

Rather than:
```example.com;host1.example.com;host2.example.com```
in the host var in /etc/dnsexit.conf. The conf file is created when running setup.py.

## Install and configure ##
```
cd
git clone https://github.com/CaptBV/dnsexit.git
cd ~/dnsexit
chmod 755 setup.py; chmod 755 ipUpdate.py
sudo ./setup.py
```

```sudo systemctl start dnsexit```
