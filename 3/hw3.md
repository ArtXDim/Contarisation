Artemiev Dima

## HOMEWORK #3

1. Update and install apt package linux

command: sudo apt update && sudo apt upgrade

![Alt text](image.png)

2. Install package 
   
command: sudo apt install apt-transport-https ca-certificates curl software-properties-common

![Alt text](image-1.png)

3. Add official GPG-key Docker:

command: curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

![Alt text](image-2.png)

4. Add repository Docker to the list package source

command: echo "deb [signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

![Alt text](image-3.png)

5. Update and install apt package linux

command: sudo apt update && sudo apt upgrade

![Alt text](image-4.png)

6. Install Docker

command: sudo apt install docker-ce

![Alt text](image-5.png)

7. Add User in docker group, to avoid using sudo to run docker commands
   
command: sudo usermod -aG docker $USER

![Alt text](image-6.png)

8. Reboot your system or run following command to apply the chenges in the current session

command: newgrp docker

![Alt text](image-7.png)

9. Check version Docker

command: docker --version

![Alt text](image-8.png)

10. Test container using image "cowsay"

command: docker run docker/whalesay cowsay Hello, Docker!

![Alt text](image-9.png)

command: docker run docker/whalesay cowsay -f elephant "Hello, Docker!"

![Alt text](image-10.png)

command: docker run docker/whalesay cowsay -f tux "Hello, Docker!"

![Alt text](image-11.png)

command: docker run docker/whalesay cowsay -f dragon "Hello, Docker!"

![Alt text](image-12.png)

command: docker run docker/whalesay cowsay -f kitty "Hello, Docker!"

![Alt text](image-13.png)

11. Create and run container

Смотрим, какие образы у нас установлены.

command: docker images

![Alt text](image-15.png)

comand: docker create ubuntu 

![Alt text](image-14.png)

command: docker ps -a

![Alt text](image-16.png)

command: docker rm 02ce2c19b859

![Alt text](image-17.png)

command: 

Run container

command: docker run -it -h ard --name gb-test ubuntu:22.10

![Alt text](image-18.png)

command: ls -l

![Alt text](image-19.png)

Создадим новую директорию в корне.

command: mkdir example

![Alt text](image-20.png)

Создадим файл "passwords.txt", добавим в него какие-либо данные и сделаем вывод файла. В контейнере не установлен текстовый редактор, но мы справимся без него.

command:  

touch passwords.txt
echo "123test" >> /exempel/password.txt

![Alt text](image-21.png)

Поработаем с внешним хранилищем

![Alt text](image-22.png)