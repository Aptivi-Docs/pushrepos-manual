---
description: How do you install this script?
---

# 📀 Installing

Installing this script is easy. To install it, follow these steps, assuming that you have either `CURL` or `wget` installed on your Linux system:

## Local and System-wide

There are two ways to install this script on your system. If you want to make this script available to all the users on your Linux system, be sure to install it on your home directory like this:

```
$ curl -fsSL https://raw.githubusercontent.com/Aptivi/pushrepos/main/pushrepos > $HOME/pushrepos
$ chmod +x $HOME/pushrepos
```

If you want to make this script available to all of the users installed, follow these two scripts as root (`sudo`):

```
$ curl -fsSL https://raw.githubusercontent.com/Aptivi/pushrepos/main/pushrepos | sudo tee /usr/local/bin/pushrepos
$ sudo chmod +x /usr/local/bin/pushrepos
```

If you prefer using wget to install the script, follow these steps:

* For local installs

```
$ wget -O$HOME/pushrepos https://raw.githubusercontent.com/Aptivi/pushrepos/main/pushrepos
$ chmod +x $HOME/pushrepos
```

* For system-wide installs

```
$ sudo wget -O/usr/local/bin/pushrepos https://raw.githubusercontent.com/Aptivi/pushrepos/main/pushrepos
$ sudo chmod +x /usr/local/bin/pushrepos
```

{% hint style="info" %}
For MinGW, WSL, and Git Bash installs, only the local install is supported.
{% endhint %}
