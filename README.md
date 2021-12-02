# DockerCompose

## ZADANIE NR 2 Budowa środowiska do rozwoju i uruchamiania aplikacji webowych.

Budowa stacku LEMP z czerema usługami: 
- NGINX
- PHP-FPM
- MySQL
- PhpMyAdmin

Stack uruchamiamy poleceniem: docker-compose up -d

Kontener NGINX uruchamia stronę internetową napisaną w języku PHP, jej kod znajduje się w folderze src/.
Po wpisaniu w przeglądarkę "localhost' pojawi się strona pokazująca napis "it works"
![image](https://user-images.githubusercontent.com/73463891/144509506-b5acfe0f-b115-4cfe-a608-078745b93fef.png)


Serwer phpMyAdmin działa na porcie 6001, umożliwia zalogowanie się do niego oraz tworzy testową bazę o nazwie "testdb"
Po wpisaniu w przeglądarkę "localhost:6001" należy się zalogować
![image](https://user-images.githubusercontent.com/73463891/144510226-023a1e55-38a0-4ec0-9e24-1f71d796842a.png)


Utworzono bazę "testdb" za pomocą polecenia w docker-compose.yml "MYSQL_DATABASE: 'testdb'", która będzie
stworzona podczas uruchamiania obrazu:
![image](https://user-images.githubusercontent.com/73463891/144510322-df14b2e7-c752-4daa-86e0-8dd3e5a0c6da.png)


struktura projektu:

![image](https://user-images.githubusercontent.com/73463891/144512902-4e5a5b64-a05c-434e-8ed9-f671f1fc1e6a.png)

W pliku php.conf znajduje się konfiguracja serwera php, która wskazuje, gdzie znajduje się folder 
zawierający kod aplikacji.



