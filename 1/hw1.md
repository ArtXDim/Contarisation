Артемьев Дмитрий Владимирович 

## Homework 1

1. sudo apt-get upgrade -  downloads and installs the updates for each outdated package and dependency on your system

![Alt text](image.png)

2. Create folder  "testfolder":
mkdir testfolder

![Alt text](image-2.png)

3. Copy the shell executable /bin/bash in folder "testfolder/bin":
cp /bin/bash testfolder/bin

![Alt text](image-1.png)

4. Create needed directory "testfolder/lib" и "testfolder/lib64":

    mkdir testfolder/lib

    mkdir testfolder/lib64

![Alt text](image-3.png)

5. Copy needed lib in folder "testfolder/lib" and "testfolder/lib64".

    cp /lib/x86_64-linux-gnu/libtinfo.so.6 testfolder/lib

    cp /lib/x86_64-linux-gnu/libc.so.6 testfolder/lib

    cp /lib64/ld-linux-x86-64.so.2 testfolder/lib64/

![Alt text](image-4.png)

6. Start comand "chroot" for change root folder:
   
    chroot testfolder /bin/bash

![Alt text](image-5.png)

1. ip netns help — view help command netns
   
![Alt text](image-6.png)

1. ip a view IP adress

![Alt text](image-7.png)

9. Ps aux - start a tool to monitor processes running on your Linux system

![Alt text](image-8.png)




