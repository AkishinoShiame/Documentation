# CUDA-8-and-ubuntu-1604-setup
<br />
1. Install ubuntu 16.04.1 LTS<br />
<br />
2. fix the issue shows below and reboot the system<br />
<br />
==============================<br />
<br />
It is known that the version of Spyder is raising this error: ValueError: unknown locale: XXXXX, which doesn’t let it start correctly.<br />
<br />
To fix it you will have to set these environment variables in your ~/.profile (or ~/.bashrc) manually:<br />

``` Shell
export LANG=en_US.UTF-8
export LC_ALL=en_US.UTF-8
```

==============================<br />
<br />
3. install spyder by:<br />
``` Shell
sudo apt-get install spyder
```
<br />
4. exec the spyder for first time setup<br />
<br />
5. install gcc 4.4 for the capability on CUDAtoolkit 8 RC<br />
<br />
==============================<br />
Getting g++-4.4 / gcc-4.4 : ```sudo gedit /etc/apt/sources.list```.
<br />
Then add two new lines to the file :<br />
``` Shell
deb [URL] trusty main universe
deb [URL] trusty-updates main universe
```
My example :<br />
``` Shell
deb http://dk.archive.ubuntu.com/ubuntu/ trusty main universe
deb http://dk.archive.ubuntu.com/ubuntu/ trusty-updates main universe
```
Run `sudo apt-get update`, and you can install gcc-4.4 : `sudo apt-get install g++-4.4`.
==============================<br />
<br />
6. download the nvidia CUDAtoolkit from Website<br />
<br />
==============================
Installation Instructions:<br />
<br />
``` Shell
  sudo dpkg -i cuda-repo-ubuntu1604-8-0-rc_8.0.27-1_amd64.deb
  sudo apt-get update
  sudo apt-get install cuda

```
==============================<br />
<br />
7. donlowd and copy cuDNN5 from website<br />
<br />
==============================<br />
Installation Instructions:<br />
<br />
``` Shell
  sudo cp -P cuda/include/* /usr/local/cuda/include
  sudo cp -P cuda/lib64/* /usr/local/cuda/lib64
  sudo cp -P cuda/include/* /usr/local/cuda-8.0/include
  sudo cp -P cuda/lib64/* /usr/local/cuda-8.0/lib64
```
==============================<br />
<br />
8. install driver<br />
<br />
==============================<br />
Now for the fix<br />
<br />
    Log into your account in the TTY.
    Run `sudo apt-get purge nvidia-*`.
    Run `sudo add-apt-repository ppa:graphics-drivers/ppa` and then `sudo apt-get update`.
    Run `sudo apt-get install nvidia-current nvidia-settings`.
    Reboot and your graphics issue should be fixed.
<br />
==============================<br />
<br />
9. fix the error 'Possible missing firmware' (not always needed)<br />
<br />
==============================<br />
https://01.org/linuxgraphics/intel-linux-graphics-firmwares
``` Shell
  tar xf <filename>.tar.bz2
  cd <foldername>
  sudo sh install.sh
```
==============================<br />
<br />
10. install tensorflow with GPU<br />
<br />
==============================<br />
<br />
``` Shell
  sudo apt-get install python-pip python-dev
  export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow-0.10.0rc0-cp27-none-linux_x86_64.whl
  sudo pip install --upgrade $TF_BINARY_URL
```
<br />
==============================<br />
<br />
11. finished!!  reboot & enjoy using it.<br />
<br />
==============================<br />
<br />
``` Shell
sudo reboot
```
<br />
==============================<br />
<br />
