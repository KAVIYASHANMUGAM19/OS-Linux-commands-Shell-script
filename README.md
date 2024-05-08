# NAME : KAVIYA S
# REGISTER NUMBER : 212223040090
# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
## OUTPUT
![Screenshot 2024-02-20 194753](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/abd6f097-d463-4c21-bda8-265e66f7d69d)


cat < file2
## OUTPUT
![Screenshot 2024-02-20 194805](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/8819a597-8b32-4e67-9d2f-27e785b0e8e5)



# Comparing Files
cmp file1 file2
## OUTPUT
![Screenshot 2024-02-20 194814](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/73b4794d-dca6-48b4-bb8e-15e26bebf6e0)

 
comm file1 file2
## OUTPUT
![Screenshot 2024-02-20 194907](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/91b831e1-f845-403e-91da-30da74b0f4f6)


 
diff file1 file2
## OUTPUT
![Screenshot 2024-02-20 194934](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/e6f79a39-b3c4-49ee-8cec-4b0ac7f7b27a)




### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```


cut -c1-3 file11
## OUTPUT
![Screenshot 2024-02-20 195201](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/eda20510-fdbf-41a5-8429-4e5e241ad469)





cut -d "|" -f 1 file22
## OUTPUT
![Screenshot 2024-02-20 195313](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/083a9024-3834-46c6-86ce-c15a6b5f7e7d)




cut -d "|" -f 2 file22
## OUTPUT
![Screenshot 2024-02-20 195344](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/6c24c350-f836-48b3-9ebc-56267c8d8d9d)



cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
 
grep Hello newfile 
## OUTPUT
![Screenshot 2024-02-20 195647](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/dcab35af-fd11-42a6-8e9f-a26bf0ef3aa5)




grep hello newfile 
## OUTPUT
![Screenshot 2024-02-20 195708](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/9910a9f3-8261-4b03-87a4-9b7c1862437c)





grep -v hello newfile
## OUTPUT
![Screenshot 2024-02-20 195728](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/7867b87e-7154-4c77-a9a2-420d82eaeaa3)




cat newfile | grep -i "hello"
## OUTPUT
![Screenshot 2024-02-20 195801](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/c0c299e1-1bc4-405a-88f7-344a33c7d591)





cat newfile | grep -i -c "hello"
## OUTPUT
![Screenshot 2024-02-20 195821](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/3179cd58-3720-4b6f-ada2-2634ec03d030)



grep -w -n world newfile   
## OUTPUT
 ![Screenshot 2024-02-21 132234](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/a46b4545-2713-4e53-935c-d28b586fb419)



cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
egrep -w 'Hello|hello' newfile 
## OUTPUT
![Screenshot 2024-02-20 203602](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/94a3d21e-7ce4-45f2-a099-677bab50c784)




egrep -w '(H|h)ello' newfile 
## OUTPUT
![Screenshot 2024-02-20 203631](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/ea422e83-17f3-4f94-a140-e731bf708ad5)




egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
![Screenshot 2024-02-20 203655](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/1e9c3896-3183-40c1-8323-c23b2bef1980)





egrep '(^hello)' newfile 
## OUTPUT
![Screenshot 2024-02-20 203713](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/92391847-ee06-44bf-ade7-93f5229d503a)




egrep '(world$)' newfile 
## OUTPUT
![Screenshot 2024-02-20 203737](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/81f5f28f-6854-47b5-bb21-e3ff5cae44c9)




egrep '(World$)' newfile 
## OUTPUT
![Screenshot 2024-02-20 203822](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/a914f62d-e80f-4d12-a146-d0421a1e426d)



egrep '((W|w)orld$)' newfile 
## OUTPUT
![Screenshot 2024-02-20 203856](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/122cc750-cef2-4037-8a25-5873a8df50fc)




egrep '[1-9]' newfile 
## OUTPUT
![Screenshot 2024-02-20 203937](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/b685d6ac-28f9-4709-ae5e-070e798df656)




egrep 'Linux.*world' newfile
## OUTPUT
![Screenshot 2024-02-20 204002](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/7cbce219-7807-4f85-b655-fd1ee178f2ee)



egrep 'Linux.*World' newfile 
## OUTPUT
![Screenshot 2024-02-20 204030](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/aa978851-0dba-4847-a8ab-6df23ef9221d)



egrep l{2} newfile
## OUTPUT
![Screenshot 2024-02-20 204048](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/275de889-5eff-4bf6-8d7b-e0f8cad5acb9)




egrep 's{1,2}' newfile
## OUTPUT
![Screenshot 2024-02-20 204114](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/d5aef624-70a1-4dbb-8288-674cd17562f9)



cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```


sed -n -e '3p' file22
## OUTPUT
![Screenshot 2024-02-20 204247](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/9493602a-ca43-4ab4-ac87-4e051e1d8e02)




sed -n -e '$p' file22
## OUTPUT
![Screenshot 2024-02-20 204325](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/59f01d0a-c4b0-4eb0-a499-3621b8792b74)




sed  -e 's/Ram/Sita/' file22
## OUTPUT
![Screenshot 2024-02-20 204349](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/61316a35-75ba-41e0-9a6a-071e08008fdc)




sed  -e '2s/Ram/Sita/' file22
## OUTPUT
![Screenshot 2024-02-20 204421](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/59b81214-b88f-49ee-bb27-343f9aab68f9)



sed  '/tom/s/5000/6000/' file22
## OUTPUT
![Screenshot 2024-02-20 204456](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/7ccca9a6-5061-41d8-a5c5-b7f39a46415b)




sed -n -e '1,5p' file22
## OUTPUT
![Screenshot 2024-02-20 204521](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/982d6ca7-a54b-43a2-b7ed-e38fcea7fcb0)




sed -n -e '2,/Joe/p' file22
## OUTPUT
![Screenshot 2024-02-20 204542](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/9f4470ae-3336-4392-a35d-0eeef53b803a)





sed -n -e '/tom/,/Joe/p' file22
## OUTPUT
![Screenshot 2024-02-20 204607](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/0ae9aa78-f46e-4f25-867a-fceae7242760)




seq 10 
## OUTPUT
![Screenshot 2024-02-20 204630](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/7487e0a4-6962-4715-9056-a8e9c1e77dc8)




seq 10 | sed -n '4,6p'
## OUTPUT
![Screenshot 2024-02-20 204737](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/f6917505-cddb-4c99-82a7-34b34acb7a94)




seq 10 | sed -n '2,4p'
## OUTPUT
![Screenshot 2024-02-20 204857](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/15e0601b-3904-40cf-a36f-4dd58d75d8bf)




seq 3 | sed '2a hello'
## OUTPUT
![Screenshot 2024-02-20 204922](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/b402483f-a8d3-4e37-8c77-36dc85ec6f0c)



seq 2 | sed '2i hello'
## OUTPUT
![Screenshot 2024-02-20 204943](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/333e1b97-d43f-41cf-93e6-f5e625ab6c1f)


seq 10 | sed '2,9c hello'
## OUTPUT
![Screenshot 2024-02-20 205010](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/44eeb1cd-1601-4410-90ac-c91f1110789b)


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
![Screenshot 2024-02-20 205044](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/e3cf06e6-452d-4bf1-a1fd-edbe10d3d70f)



sed -n '2,4{s/$/*/;p}' file23
## OUTPUT
![Screenshot 2024-02-20 205108](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/b779b280-93c6-4829-9bd1-3b92faafea28)


#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT
![Screenshot 2024-02-20 205201](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/c5be9e44-1805-4c71-92cb-2bf97c95817d)


cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT
![Screenshot 2024-02-20 205401](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/32f271ff-9dd3-44ef-9ac2-cd9734c12556)



#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
![Screenshot 2024-02-20 205513](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/ed5bc641-d754-4c2d-9e0f-e412304de495)

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
## OUTPUT
![Screenshot 2024-02-20 205622](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/cd0af4f1-9f99-45fc-846f-3299455076a3)


 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
![Screenshot 2024-02-20 205644](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/c6e8385d-c038-455f-b324-261e38909180)



#Backup commands
tar -cvf backup.tar *
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/a4b0bdd9-700a-4908-8f4c-3013180ee07d)


mkdir backupdir
 
mv backup.tar backupdir
 
tar -tvf backup.tar
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/b90c0851-c29e-4958-8f1e-33b9b2365ecd)


tar -xvf backup.tar
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/6b8b371b-c659-47ba-8de8-9aadf19e70fb)

gzip backup.tar
## OUTPUT

 
gunzip backup.tar.gz
## OUTPUT
l
 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT


cat <cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT

 echo $?
## OUTPUT
![Screenshot 2024-02-24 124040](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/b805ec0c-8411-477a-9048-a23898df4aac)


echo $?
## OUTPUT 
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/71413be1-6c2a-4788-99a2-17097ce6411e)

./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
![Screenshot 2024-02-24 124040](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/1f8c0619-c808-42ca-9e25-b5f3d265dfc7)

 
abcd
 
echo $?
 ## OUTPUT
 ![Screenshot 2024-02-24 124040](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/e892d510-6f36-449d-8d9c-774d61ee4cd9)



 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```

chmod 755 strcomp.sh
./strcomp.sh 
## OUTPUT
![Screenshot 2024-02-21 142742](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/1dcf04e3-920f-45a0-a507-79031af00358)


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
![Screenshot 2024-02-26 101731](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/29523d35-0705-4d57-ac87-e4f37d754330)



# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT
![Screenshot 2024-02-26 104711](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/36ceb7e6-c177-4ee8-9e14-746e043ca50e)




# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
## OUTPUT
![Screenshot 2024-02-24 130225](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/1d71e934-177b-4312-bef1-0060dc979c68)


# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
## OUTPUT
![Screenshot 2024-02-26 104711](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/0cd9ee3d-1ca7-49a9-adf7-883928ee1e81)



# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT
![Screenshot 2024-02-24 131230](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/092499f2-edf1-4dff-9d29-bf258a7c5b1c)



# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh

$ ./ifcompound.sh 
## OUTPUT
![Screenshot 2024-02-24 131345](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/764b3737-3cfa-4f2d-8da1-cb1d54a03442)



# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 

$ ./casecheck.sh

## OUTPUT
![WhatsApp Image 2024-02-28 at 14 42 48_a8f5e1a3](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/c43bcf4d-2d40-4eae-938f-29597afb6a75)

 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh

$ ./whiletest.sh

## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/6455f361-51b5-4016-b6ab-c088d0e509e1)

 
 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh

$ ./untiltest.sh

## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/74f2cbc2-06e8-4160-bd11-bc7564423c67)

 
 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh

$ ./forin1.sh
## OUTPUT
![Screenshot 2024-02-26 111416](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/5dc4f767-d02a-4202-9095-de2fd4dd0a6e)


cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh

$ ./forin2.sh 
## OUTPUT
![Screenshot 2024-02-26 111557](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/ddfb35d7-07c6-4bcc-8238-28534dbac643)

 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
## OUTPUT
![Screenshot 2024-02-26 111812](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/ef3e5a09-7495-46e5-b762-e3223388d56a)

 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

$ ./forinfile.sh
## OUTPUT
![Screenshot 2024-02-26 112022](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/b8225fa7-99dc-450f-924d-dd85159643f9)

cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT
![Screenshot 2024-02-26 113801](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/89247b46-9dd3-4a6f-87db-e2e52bdba71b)



cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/dab9024f-0c7b-475a-a76a-d2f6c5122dcf)

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh

$ ./forctype1.sh 
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/1e2ea90f-1567-4b78-a2a7-fbc3dbb60847)


cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT
 ![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/2a9a2a20-8e81-43c3-9098-25596c2ec202)


 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
$ chmod 755 forbreak.sh

$ ./forbreak.sh 
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/a344b040-b848-456b-9c6b-c215be68360a)

 
cat forcontinue.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
$ chmod 755 forcontinue.sh

$ ./forcontinue.sh 
## OUTPUT
 ![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/4c006095-6327-47b1-a7e0-6f7659400433)

cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
$ chmod 755 exread.sh 

$ ./exread.sh 
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/9bd5e462-c2f2-4952-a257-bcfc7524c8bd)


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

$ ./exread1.sh
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/27963d9a-955f-4e6d-b39f-c8338b845b45)


 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
 ./funcex.sh 
 ## OUTPUT
 ![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/aa488045-5fad-45c2-8ee4-f66d9aea7fe0)

cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777  argshift.sh 

$ ./argshift.sh 1 2 3
## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/418678e9-67f5-4189-8919-c3f20cfc3614)
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]}
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
 # echo each element in array  
# for loop 


```
$ chmod 777 argshift.sh

$ ./argshift.sh 1 2 3

## OUTPUT
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/0e0ef1a4-9bf9-46b8-a7b4-bc559ad3c5f6)

 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
 ./argshift.sh 1 2 3
 ## OUTPUT
![Screenshot 2024-02-29 132945](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/5ace63dd-b541-437d-9b1a-23edd7709e62)



 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghjGIG
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
![Screenshot 2024-02-28 201128](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/6d52873f-ebaf-4955-af80-e829cf427eda)
  


cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
$ chmod 755 palindrome.sh

$ ./palindrome.sh

## OUTPUT :
![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/20663c0d-8fb4-4c15-ab4d-90da9a5dd0c3)

![image](https://github.com/KAVIYASHANMUGAM19/OS-Linux-commands-Shell-script/assets/155141139/47e21b1f-cf09-4ba9-9fcd-4d8bdb9d84c5)




# RESULT:
The Commands are executed successfully.
