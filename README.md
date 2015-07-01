# What is Agora-Project

Agora-Project is a collaborative workspace complete and intuitive. This application is accessible anywhere and 
anytime via a web browser. Several languages are available.

Many modules are integrated into the workspace :
* File Manager
* Personal Calendar and Resource Calendar
* Forum
* Task Manager
* Directory of contacts
* Newsletters
* Bookmarks
* Space users
* Dashboard
* LiveCounter and Messenger
* Search

For more information you can visit upstream project : https://www.agora-project.net

# How to use this image

Agora need a mysql database :

```docker run -d --name agora-mysql -e MYSQL_ROOT_PASSWORD=password mysql```

Finally launch agora container linked to mysql :

```docker run -d -P --name agora --link agora-mysql:mysql cquad/agora```
