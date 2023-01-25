 #Create 10 files and 10 directories
 Answer:
        root@logesh-Vm:/home/logesh# touch file{1..10}

        root@logesh-Vm:/home/logesh# mkdir fold{1..10}

        root@logesh-Vm:/home/logesh# ls

        file1  file10  file2  file3  file4  file5  file6  file7  file8  file9  fold1  fold10  fold2  fold3  fold4  fold5  fold6  fold7  fold8  fold9



#Create 2 new users called "guviuser" & "zenuser
Answer:
       root@logesh-Vm:/home/logesh# useradd guviuser

       root@logesh-Vm:/home/logesh# useradd zenuser
       


#Modify the permissions where, * the first 5 files & directories must have ownership as 'guviuser' with read,write,execute permissions for everyone 
Answer:
       root@logesh-Vm:/home/logesh# chown guviuser file{1..5}

       root@logesh-Vm:/home/logesh# chmod 755 file{1..5}  

       root@logesh-Vm:/home/logesh# chown guviuser fold{1..5}

       root@logesh-Vm:/home/logesh# chmod 755 fold{1..5}
       


#The last 5 files & directories must have ownership as 'zenuser' with only read permission to only the owner  
Answer:
       root@logesh-Vm:/home/logesh# chown zenuser file{6..10}

       root@logesh-Vm:/home/logesh# chmod 400 file{6..10}

       root@logesh-Vm:/home/logesh# chown zenuser fold{6..10}

       root@logesh-Vm:/home/logesh# chmod 400 fold{6..10}
       
       
FILE PERMISIONS 
          root@logesh-Vm:/home/logesh# ls -l file{1..10}

 -rwxr-xr-x 1 guviuser root 0 Jan 25 20:07 file1
 -r-------- 1 zenuser  root 0 Jan 25 20:07 file10
 -rwxr-xr-x 1 guviuser root 0 Jan 25 20:07 file2
 -rwxr-xr-x 1 guviuser root 0 Jan 25 20:07 file3
 -rwxr-xr-x 1 guviuser root 0 Jan 25 20:07 file4
 -rwxr-xr-x 1 guviuser root 0 Jan 25 20:07 file5
 -r-------- 1 zenuser  root 0 Jan 25 20:07 file6
 -r-------- 1 zenuser  root 0 Jan 25 20:07 file7
 -r-------- 1 zenuser  root 0 Jan 25 20:07 file8
 -r-------- 1 zenuser  root 0 Jan 25 20:07 file9









