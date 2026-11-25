# Варианты запуска

## Встроенный в Spring Boot сервер Tomcat
По умолчанию приложение не требует подключения внешнего сервера. Запускается src/main/java/web/App.java#main()

## Внешний сервер Tomcat 10+
1. src/main/java/web/App.java - комментируем аннотацию @SpringBootApplication
2. src/main/java/web/AppTomcat.java - раскомментируем аннотацию @SpringBootApplication
3. pom.xml: раскомментируем packaging war и зависимость spring-boot-starter-tomcat
4. обновляем проект Maven