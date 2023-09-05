Artemiev Dima

## HOMEWORK #5

1.  Update all packages

command:  sudo apt update && sudo apt upgrade

![Alt text](image.png)

2. Create folder for progect

command: mkdir progect

![Alt text](image-1.png)

3. Create in folder yml-file with name docker-compose.yml

command: touch docker-compose.yml

![Alt text](image-2.png)

![Alt text](image-4.png)

4. Install docker-compose

command: apt install docker-compose

![Alt text](image-3.png)

5. Create and run project

command: docker-compose up -d

![Alt text](image-5.png)

6. Check a create two containers

command: docker-compose ps

![Alt text](image-6.png)

7. Open page http://localhost:8081

![Alt text](image-7.png)

8. Вбиваем в форму имя пользоваля root и пароль, который мы указывали в докер-компоуз файле в переменных среды - test123, и входим в Adminer. Видим, что используется база данных MariaDB.

![Alt text](image-8.png)