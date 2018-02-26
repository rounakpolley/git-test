# Kalyani Government Engineering College
### Department of Computer Science & Engineering
### OS-LAB : CS-693

#### Name      : Rounak Polley
#### Roll      : 10200115033
#### Group No. : 

## Lab assignment: 1

##### >_ Starting point after loggin in a super-user
``` powershell
[root@localhost RounakPolley]# pwd
/home/student/RounakPolley
```
##### 1. Create two sub directories teacher and students under college directory
``` powershell
[root@localhost RounakPolley]# mkdir College
[root@localhost RounakPolley]# cd College
[root@localhost College]# mkdir student
[root@localhost College]# mkdir teacher
[root@localhost College]# ls -l
total 8
drwxr-xr-x. 2 root root 4096 Feb 26 11:55 student
drwxr-xr-x. 2 root root 4096 Feb 26 11:51 teacher
```
##### 2. In student sub directory create a file course.txt
``` powershell
[root@localhost College]# cd student
[root@localhost student]# touch course.txt
[root@localhost student]# vi course.txt
```
##### 3. show the contents of the file course.txt
``` powershell
[root@localhost student]# cat course.txt
OS LAB : CS 693, 3rd Year, 2nd Semester
Group No. :
Name - Machine_no
Rounak Polley - C092
Rounak Mukeerjee - C093
Rumeet Prasad - C105
Ritik Raj - NA
```
##### 4. Move course.txt to teacher subdirectory
``` powershell
[root@localhost student]# mv student/course.txt teacher/
```
##### 5. Copy the content of course.txt to newcourse.txt
``` powershell
[root@localhost student]# cd ..
[root@localhost College]# cp teacher/course.txt student/newcourse.txt
[root@localhost College]# cd student
[root@localhost student]# cat newcourse.txt
OS LAB : CS 693, 3rd Year, 2nd Semester
Group No. :
Name - Machine_no
Rounak Polley - C092
Rounak Mukeerjee - C093
Rumeet Prasad - C105
Ritik Raj - NA
```
##### After completing the steps
``` powershell
[root@localhost student]# cd ..
[root@localhost College]# ls -R
.:
student  teacher

./student:
newcourse.txt  test.txt

./teacher:
course.txt
[root@localhost College]# exit
```
