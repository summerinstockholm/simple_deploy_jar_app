1. Сначала установим open-jdk: apt install default-jdk
2. Установим сборщик maven: apt install maven
3. Установим tomcat: apt install tomcat9
4. Установить git: apt install git
5. Клонирую репу из https://github.com/ExeterBScDTS/simple-servlet
git clone https://github.com/ExeterBScDTS/simple-servlet.git
6. Перейти в директорию с исходным кодом: cd simple-servlet и собираем проект через maven: mvn package
По итогу получим артефакт: /home/catware/simple-servlet/target/simple-servlet-0.1.war
переходим в директорию /home/catware/simple-servlet/target: cd target
7. Запуск в томкате через копирование в рабочую директорию томката по умолчанию: cp simple-servlet-0.1.war /var/lib/tomcat9/webapps/ 
8. По итогу готовое приложение лежит в /var/lib/tomcat9/webapps/simple-servlet-0.1 - сюда распаковался варник.
9. http://84.201.179.251:8080/simple-servlet-0.1/ все получилось
