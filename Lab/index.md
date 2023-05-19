# ECRYPTFS Lab

<p align="justify">

### **What is eCryptFS?**

ECRYPTFS (Enterprise Cryptographic Filesystem) is an open-source file-based encryption tool for
Linux, which provides on-the-fly encryption for individual files or directories.

It is designed to be transparent to the user, allowing them to access and use encrypted files and
directories just like normal files and directories.

With this information, we are set to dive into the installation and use of eCryptFS.

</p>
<hr> 

## installation Steps 


**Step 1: Install eCryptFS on Linux**

eCryptFS is available in many Linux distros’ default repositories and can be installed with the below commands:

```shell
sudo dnf install https://www.elrepo.org/elrepo-release-9.el9.elrepo.noarch.rpm
sudo yum install epel-release
sudo yum install ecryptfs-utils
```

**Step 2: Encrypt Directories With eCryptfs On Linux**

With eCryptfs installed on your Linux system, we are set to encrypt directories. the general syntax to encrypt a directory with eCryptfs is:

```
mount -t ecryptfs [source directory] [Destintaion directory] -o [options]
```

You are required to replace the Destination directory with your own directory. Let’s take a practical example using the directory `/nada` on my system. The command here will be:

```
sudo mount -t ecryptfs nada/ nada/
```
