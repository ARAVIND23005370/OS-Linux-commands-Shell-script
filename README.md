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
![Screenshot from 2024-02-26 21-11-54](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/a5d5e3e9-f2a8-49bf-843f-90b65a9c5d52)




cat < file2
## OUTPUT
![Screenshot from 2024-02-26 21-12-30](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/ef8ad9dd-df59-4ea3-8bf6-f5bc52c2e120)


# Comparing Files
cmp file1 file2
## OUTPUT
 ![Screenshot from 2024-02-26 21-13-11](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/f632b9d6-49d5-4b31-89b1-46ff43182a70)

comm file1 file2
 ## OUTPUT
![Screenshot from 2024-02-26 21-13-34](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/fffb2c7d-1084-4131-9ad9-e2b7a7631dd1)

 
diff file1 file2
## OUTPUT
![Screenshot from 2024-02-26 21-13-49](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/bde53dcf-f7b2-466c-aab5-338b8c07857d)


#Filters

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


![Screenshot from 2024-02-26 21-19-08](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/d779b102-f3da-48e6-bfd0-d4472e7e78b3)


cut -d "|" -f 1 file22
## OUTPUT
![Screenshot from 2024-02-26 21-19-16](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/2d87e99c-cf5a-4e5d-8f03-2ce367c6312a)



cut -d "|" -f 2 file22
## OUTPUT
![Screenshot from 2024-02-26 21-19-24](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/3a822617-cff2-46ad-ba8b-1c856c9f5094)


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
![Screenshot from 2024-02-26 21-33-01](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/20f02172-00ec-4acf-837f-7599e986b465)




grep hello newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-33-09](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/f7a0151e-da7c-46ac-9d30-685298d26bd2)




grep -v hello newfile 
## OUTPUT

![Screenshot from 2024-02-26 21-33-19](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/ea09b0c0-1297-4f74-b31a-069987b08546)


cat newfile | grep -i "hello"
## OUTPUT

![Screenshot from 2024-02-26 21-33-43](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/440d295e-858e-4b0c-a45a-585671a5643b)



cat newfile | grep -i -c "hello"
## OUTPUT
![Screenshot from 2024-02-26 21-34-14](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/60204a48-69f8-49ba-a91e-cc5a1ee7d15d)




grep -R ubuntu /etc
## OUTPUT

![Screenshot from![Screenshot from 2024-02-26 21-35-28](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/7db72f8c-55d3-469c-9ca0-8db4ba28075c)
 2024-02-26 21-35-08](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/3afa9d37-657a-4584-a36a-94dce3118e9e)
![Screenshot from 2024-02-26 21-35-48](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/fee699da-bb0b-449d-9e6b-dac102c12359)
![Screenshot from 2024-02-26 21-36-03](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/e3c8955e-79ab-439a-8f56-3ee70902067a)
![Screenshot from 2024-02-26 21-36-18](https://github.com/ARAVIND23005370/OS-Linux-comman![Screenshot from 2024-02-26 21-36-26](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/a01e0575-79f1-405d-81c2-853eedefd450)
ds-Shell-script/assets/148514836/11afb0f8-9145-4fee-8ed0-50bb159d5349)
![Screenshot from 2024-02-26 21-36-29](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/589aa3c8-3ec3-4efa-b088-b8621f027d6f)
![Screenshot from 2024-02-26 21-36-47](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/40d26fc9-12c2-4437-9829-5d74ab241250)


grep -w -n world newfile   
## OUTPUT
![Screenshot from 2024-02-26 21-38-31](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/adda4128-b6b0-41da-8f7b-8221c2806ea8)


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
![Screenshot from 2024-02-26 21-38-31](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/f52cd63a-c543-4ebb-b05a-7d68d976dac9)



egrep -w '(H|h)ello' newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-38-54](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/0d733c2c-7b7c-45af-b5da-e9be7dfc2599)



egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-44-04](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/b208ce48-1bea-43d7-a502-df2678819e4a)




egrep '(^hello)' newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-44-17](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/cb17b70f-a86a-44ee-b884-180d4e559e0a)



egrep '(world$)' newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-44-26](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/4c517470-2528-48cd-93a5-eeb499acde40)



egrep '(World$)' newfile 
## OUTPUT

![Screenshot from 2024-02-26 21-44-42](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/329cc736-d1de-454e-9bfb-c0f7dfdd9c3c)

egrep '((W|w)orld$)' newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-44-52](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/5b0ba828-415f-4fcf-9b93-8adb705424b8)



egrep '[1-9]' newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-48-52](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/080d3bb0-3cc1-4fa7-adb4-26b8091dcc27)



egrep 'Linux.*world' newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-49-15](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/4367ebaf-949f-4164-8d8f-a2a42e072b83)


egrep 'Linux.*World' newfile 
## OUTPUT
![Screenshot from 2024-02-26 21-49-28](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/2a8f1edb-2d44-4b69-aa8d-b6e99d0e0fc9)


egrep l{2} newfile
## OUTPUT
![Screenshot from 2024-02-26 21-49-37](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/fe33c037-c486-4263-ae0d-e6f7d42c1bf4)



egrep 's{1,2}' newfile
## OUTPUT 
![Screenshot from 2024-02-26 21-49-45](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/330e4496-476e-4240-baa2-db6dcea4eca2)



cat > file23
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


sed -n -e '3p' file23
## OUTPUT
![Screenshot from 2024-02-26 21-49-53](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/05536e22-1278-4e51-9de5-248c33ed7716)



sed -n -e '$p' file23
## OUTPUT
![Screenshot from 2024-02-26 21-50-02](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/80490ec2-f180-44a4-8efc-62f32f3d5ada)



sed  -e 's/Ram/Sita/' file23
## OUTPUT
![Screenshot from 2024-02-26 21-54-30](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/b3d574e2-26a7-4f35-bb3a-364df2577906)



sed  -e '2s/Ram/Sita/' file23
## OUTPUT

![Screenshot from 2024-02-26 21-54-37](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/cafb553e-06cb-4cd5-b674-8438cb1cb580)


sed  '/tom/s/5000/6000/' file23
## OUTPUT
![Screenshot from 2024-02-26 21-54-46](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/69a0e111-f53b-444a-ad5a-99ecbfa055c6)




sed -n -e '1,5p' file23
## OUTPUT
![Screenshot from 2024-02-26 21-54-51](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/3d908abd-1e87-4080-9570-66640602d967)



sed -n -e '2,/Joe/p' file23
## OUTPUT

![Screenshot from 2024-02-26 21-54-58](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/fcba775d-fad3-4d1f-84e0-2bbf0858e69d)



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT
![Screenshot from 2024-02-26 21-55-21](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/55ca1030-5b9d-4f41-a6cf-cfe5e2dccbb5)



seq 10 
## OUTPUT
![Screenshot from 2024-02-26 22-06-50](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/d468080e-d820-4557-9742-a9178109a272)



seq 10 | sed -n '4,6p'
## OUTPUT
![Screenshot from 2024-02-26 22-06-58](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/ec610fd5-440b-4d72-9422-363939f3116d)



seq 10 | sed -n '2,~4p'
## OUTPUT

![Screenshot from 2024-02-26 22-07-07](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/6197979b-c02c-42a4-b28a-4995c5501d9a)


seq 3 | sed '2a hello'
## OUTPUT
![Screenshot from 2024-02-26 22-07-12](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/367cf745-651d-4ef8-b335-fc80713c8df4)



seq 2 | sed '2i hello'
## OUTPUT
![Screenshot from 2024-02-26 22-07-21](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/ea91d0ec-cf36-44eb-b689-bd3d750abd3b)


seq 10 | sed '2,9c hello'
## OUTPUT
![Screenshot from 2024-02-26 22-07-50](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/a3c8b95d-6058-43dd-b621-407907eee69b)


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
![Screenshot from 2024-02-26 22-08-14](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/44ad5709-fae0-46b0-ae61-cbd2abac8948)



sed -n '2,4{s/$/*/;p}' file23


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
![Screenshot from 2024-02-26 22-13-05](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/0b04d9d3-5267-467f-8597-febc820f601e)


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

![Screenshot from 2024-02-26 22-13-18](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/dfc4e171-e9c0-4a42-a5e1-f47baa0f5b0c)


#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
![Screenshot from 2024-02-26 22-13-24](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/069c07e2-78b3-4c29-8b36-c7a715a2ce26)

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
![Screenshot from 2024-02-26 22-19-03](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/b7b2dccb-f2e5-4ef1-ab1a-eaa07a7bd384)


 
cat urllist.tx!

t | tr -d ' ' | tr -s '.'
## OUTPUT

![Screenshot from 2024-02-26 22-19-15](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/7c9b0c21-ec32-48cc-9d4e-ad891bc0ccc1)

 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPU
![Screenshot from 2024-02-26 22-19-26](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/84612709-d695-4ade-89f7-c0221f126cd4)
T

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT
![Screenshot from 2024-02-26 22-19-32](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/b2f9e6b2-c0da-446d-a8ed-e552710b70fc)


cat < scriptest.sh 
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
![Screenshot from 2024-02-26 22-19-43](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/3d734be7-52ec-47d2-ac48-49b4433fea83)

 
ls file1
## OUTPUT
![Screenshot from 2024-02-26 22-21-52](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/ce1f6152-224b-4cdd-8e49-c6c8a849510c)

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 ![Screenshot from 2024-02-26 22-21-57](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/f3b50b11-6a30-4685-b31d-81d919c7bae3)

echo $?
## OUTPUT 
 
abcd
 
echo $?
 ## OUTPUT
![Screenshot from 2024-02-26 22-23-48](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/b81e9079-8a15-4466-b090-0d038c3e6583)


 
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
##OUTPUT



chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
![Screenshot from 2024-02-26 22-23-57](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/c90d56fa-a577-4909-8bb3-223a92ab5e05)


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
![Screenshot from 2024-02-26 22-24-13](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/46172d9c-25aa-43a9-a3b5-ddf427f16e34)

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
![Screenshot from 2024-02-26 22-27-06](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/07b81e4d-6db5-4b2f-be6d-d54e0aec2845)



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
##OUTPUT

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
##OUTPUT

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
![Screenshot from 2024-02-26 22-28-43](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/77a4b21b-510f-480f-9843-0193bc7175ef)


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
![Screenshot from 2024-02-26 22-29-02](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/25a49486-0e49-4352-9b36-808c0ca8680f)

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

## OUTPUT
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
![Screenshot from 2024-02-26 22-30-52](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/dbc88b4c-a048-43e9-a7c2-9a656c108c98)

## OUTPUT
![Screenshot from 2024-02-26 22-34-00](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/ab8345ef-a56f-4f38-b306-750391fb1c0a)


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
![Screenshot from 2024-02-26 22-36-58](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/a43cece1-32fb-418d-a57d-50a9ca2f58f1)

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
![Screenshot from 2024-02-26 22-37-10](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/88d1d916-98fc-4abd-b85e-f4834c5ff892)

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
![Screenshot from 2024-02-26 22-37-18](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/10fa8cd3-b1bd-44c4-9de0-ddc275187ef5)

 
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
## OUTPUT
![Screenshot from 2024-02-26 22-48-52](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/70434420-52f6-472c-b852-ea47edf6c74d)

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
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
 ![Screenshot from 2024-02-26 22-50-07](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/89945b91-31cc-4fa6-af94-c40f10310d77)

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

![Screenshot from 2024-02-26 22-51-26](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/af57d3ae-9ba5-4ef3-9ad3-328f5f322d01)

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT
![Screenshot from 2024-02-26 22-52-50](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/375d6f58-b23c-4b66-98d4-14691a8be87e)



$ ./exread1.sh 
 
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
## OUTPUT
 ./funcex.sh 
![Screenshot from 2024-02-26 22-54-22](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/3c2e866f-8289-47c9-884b-3f7af2b3f548)

 
 ./funcex.sh 1 2

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 ![Screenshot from 2024-02-26 22-55-00](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/158f7320-d053-4ce1-beb9-d64f0da61d38)

 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
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
## OUTPUT
 ./argshift.sh 1 2 3
 ![Screenshot from 2024-02-26 22-56-11](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/2558bec7-e2a1-4c89-b8eb-bfd3231bfbb4)

 
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
bcdfghj
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
 ![Screenshot from 2024-02-26 22-55-00](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/d7a76ce7-79f1-4d90-bc34-70d8971ee561)

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
## OUTPUT![Screenshot from 2024-02-26 22-56-11](https://github.com/ARAVIND23005370/OS-Linux-commands-Shell-script/assets/148514836/d650b2dd-29f9-4ce3-8c2b-4530881a851a)
 


# RESULT:
The Commands are executed successfully.
