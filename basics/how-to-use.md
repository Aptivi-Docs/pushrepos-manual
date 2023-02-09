---
description: How do you use this script?
---

# ❓ How to use?

Running this script is so easy, especially when you have to push a change to hundreds of repositories in your Git repository library (a directory containing your Git repositories) on the remote side.

To push a change to all the repositories on the current Git repository library, just run the script with no arguments:

```
pushrepos
```

To push a change to all the repositories on any specified directory, run the script with the relative or absolute path to the directory containing your repositories:

```
pushrepos Path/To/Repos
```

To push a change to all the repositories on specified directory with a custom commit message, run the script with the relative or absolute path to the directory containing your repositories:

```
pushrepos Path/To/Repos "General Commit Message"
```

Internally, it will call the following commands:

```
$ git -C Path/To/Repos add -A .
$ git -C Path/To/Repos commit -m "$universal_commit_msg"
$ git -C Path/To/Repos push
```

{% hint style="info" %}
Depending on the repository size and your network connection speed, it might take a while.
{% endhint %}
