# HW_10
1) В домашней директории создать home_works создать директорию lesson_10
2) В директории lesson_10 создать директорию available, в ней файлы app.conf, readme.md, app.log с произвольным содержимым
3) В директории lesson_10 создать директорию enabled, в ней создать symlink на available/app.conf
4) В директории lesson_10 создать директории logs и debug; переместить файл available/app.log в директорию logs, а в debug сделать hardlink на logs/app.log
![](https://github.com/matveyframe/Lesson_10/blob/main/mkdir%20home_works.PNG "Logo Title Text 1")
5) Добавить к вашей ВМ дополнительный диск
![](https://github.com/matveyframe/Lesson_10/blob/main/Add%20Hard%20Disk.PNG "Logo Title Text 1")
6) Посмотреть список блочных устройств (lsblk) и список смонтированных ФС (df -Th)
7) Создать на новом диске ФС типа ext4
![](https://github.com/matveyframe/Lesson_10/blob/main/lsblk%20%2B%20df%20-Th.PNG "Logo Title Text 1")
8) Создать директорию /opt/application и смонтировать в нее новый диск (монтирование должно быть постоянным, через /etc/fstab)
![](https://github.com/matveyframe/Lesson_10/blob/main/fstab.PNG "Logo Title Text 1")
9) Скопировать /opt/application все содержимое lesson_10. Должно получиться примерно такое
9) Попробовать сделать hardlink на файл $HOME/home_works/lesson_10/available/readme.md в директории /opt/application (не получится); затем сделать symlink на этот же файл
![](https://github.com/matveyframe/Lesson_10/blob/main/Symlink%20application_dir.PNG "Logo Title Text 1")
