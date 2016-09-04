## **CHATTERBOX - A customizable AJAX and PHP based simple CHAT application.**

Chatterbox is a simple web app implemented using JavaScript, MySQL and PHP for a public chat room environment. 
The chat messages are updated using Javascript. Instead of updating the whole page, only the new data is retrieved by querying the server for updates.

For a quicker setup, please import [this] file to phpmyadmin. 

### **KEY FEATURES**:
>-  A clean UI for a public chat room experience.  
>- Passwords are stored as hashed output of SHA-256 with a randomly generated salt value.
>- Login/Sign up/Log out feature added.


###**TABLE STRUCTURES**:
####Table structure for table `logs`
```
CREATE TABLE IF NOT EXISTS `logs` (
  `id` int(11) NOT NULL,
  `username` varchar(255) NOT NULL,
  `msg` longtext NOT NULL,
  `time` time NOT NULL,
  `date` date NOT NULL
) ENGINE=InnoDB AUTO_INCREMENT=286 DEFAULT CHARSET=latin1;
```
####Table structure for table `users`
```
CREATE TABLE IF NOT EXISTS `users` (
  `id` int(11) NOT NULL,
  `username` text NOT NULL,
  `password` varchar(255) NOT NULL,
  `salt` varchar(255) NOT NULL
) ENGINE=InnoDB AUTO_INCREMENT=8 DEFAULT CHARSET=latin1;
```




 

[this]:https://github.com/rahul1raman/chatterbox/blob/master/chatbox.sql


