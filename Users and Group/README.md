# Users and Group

# To see total number of users use following command

      [vagrant@localhost ~]$ ls -l /home/
      total 0
      drwx------. 4 vagrant vagrant 154 Oct 15 17:45 vagrant

# To add user use useradd command

      [vagrant@localhost ~]$ useradd suman
      -bash: /usr/sbin/useradd: Permission denied
      [vagrant@localhost ~]$ sudo useradd suman
      [vagrant@localhost ~]$ ls -l /home/
      total 0
      drwx------. 2 suman   suman    62 Oct 15 18:43 suman
      drwx------. 4 vagrant vagrant 154 Oct 15 17:45 vagrant
      [vagrant@localhost ~]$ sudo useradd tom
      [vagrant@localhost ~]$ ls -l /home/
      total 0
      drwx------. 2 suman   suman    62 Oct 15 18:43 suman
      drwx------. 2 tom     tom      62 Oct 15 18:43 tom
      drwx------. 4 vagrant vagrant 154 Oct 15 17:45 vagrant

# Also to see all the users open passwd

    [vagrant@localhost ~]$ vi /etc/passwd
    [vagrant@localhost ~]$ groupadd users
    -bash: /usr/sbin/groupadd: Permission denied]
    
# To create a group use groupadd command
      [vagrant@localhost ~]$ sudo groupadd Allusers
      [vagrant@localhost ~]$ vi /etc/group

# To add users to the seconadary group use usermod -G command and to add in primary group use usermod -g command
      [vagrant@localhost ~]$ usermod -G Allusers suman
      -bash: /usr/sbin/usermod: Permission denied
      [vagrant@localhost ~]$ sudo usermod -G Allusers suman
      [vagrant@localhost ~]$ vi /etc/group
      
# To give a password to the user use passwd command 
      [vagrant@localhost ~]$ sudo passwd suman
      Changing password for user suman.
      New password:
      BAD PASSWORD: The password is shorter than 8 characters
      Retype new password:
      passwd: all authentication tokens updated successfully.
# To switch into the user use su command and just make sure you are in suman directory not in vagrant
      [vagrant@localhost ~]$ su suman
      Password:
      [suman@localhost vagrant]$ pwd
      /home/vagrant
      [suman@localhost vagrant]$ exit
      exit
# To switch into the user directory use su and - suman command
      [vagrant@localhost ~]$ su - suman
      Password:
      Last login: Tue Oct 15 18:57:23 UTC 2019 on pts/0
      [suman@localhost ~]$ ls
      [suman@localhost ~]$ pwd
      /home/suman
      [suman@localhost ~]$
