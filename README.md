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
### 1. cat < file1
## OUTPUT
![image](https://github.com/user-attachments/assets/38959521-c43b-4341-922b-324ccdcbfe81)



### 2. cat < file2
## OUTPUT
![image](https://github.com/user-attachments/assets/65095f18-9c41-4923-ab88-832b2944a115)



# Comparing Files
### 3. cmp file1 file2
## OUTPUT
![image](https://github.com/user-attachments/assets/a484f31d-1c43-4a4b-a522-6db789085b78)



### 4. comm file1 file2
## OUTPUT
![image](https://github.com/user-attachments/assets/d3a745a9-44d5-4163-a57c-ae324ad5e0e1)


 
### 5. diff file1 file2
## OUTPUT
![image](https://github.com/user-attachments/assets/9e13a438-47c2-43a0-bc38-3f750dcce2b4)



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


### 6. cut -c1-3 file11
## OUTPUT
![image](https://github.com/user-attachments/assets/88d4d99d-c448-4024-ad68-2cecb976bb9d)



### 7. cut -d "|" -f 1 file22
## OUTPUT
![image](https://github.com/user-attachments/assets/4b20c30c-7be2-4e35-ae9f-d89b623703f3)



### 8. cut -d "|" -f 2 file22
## OUTPUT
![image](https://github.com/user-attachments/assets/57276d83-92fc-4f51-ae11-e259cfa89693)



cat > newfile 
```
Hello world
hello world
^d
````

 
### 9. grep Hello newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/f242b46b-9a00-4828-a019-66d5e20c1885)



### 10. grep hello newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/4abcd87e-1217-470c-b21d-fde0b9045616)




### 11. grep -v hello newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/0b773088-7ef6-4c5e-ad0d-7839d9cb0add)



### 12. cat newfile | grep -i "hello"
## OUTPUT
![image](https://github.com/user-attachments/assets/b5d96888-8a74-4e1e-9ee8-7e5938ab77e2)




### 13. cat newfile | grep -i -c "hello"
## OUTPUT
![image](https://github.com/user-attachments/assets/80e1601a-13d8-479a-b2e3-90247e940193)




grep -R ubuntu /etc
## OUTPUT



### 15. grep -w -n world newfile   
## OUTPUT
![image](https://github.com/user-attachments/assets/5e63c904-056d-440d-9565-951d9790590a)



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

### 16. egrep -w 'Hello|hello' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/181dee33-d68f-49b5-bc1b-687b1527e5a1)



### 17. egrep -w '(H|h)ello' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/128e21df-3b07-4d30-88ef-8db73d9da3bc)



### 18. egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/dca1f747-694e-4aa7-9704-47f91bf8e5a6)




### 19. egrep '(^hello)' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/eb799819-af91-4b1d-9959-f7ee927f451d)



### 20. egrep '(world$)' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/3b4fc7cd-39f8-4423-bf00-d45c84cd0070)



### 21. egrep '(World$)' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/f43efe8a-e266-42e6-a2ef-b17b01657071)



### 22. egrep '((W|w)orld$)' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/997d1225-d91d-45df-a9ec-2cc79133028b)



### 23. egrep '[1-9]' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/c0b20a8c-2737-428f-800b-2a318e16b451)



### 24. egrep 'Linux.*world' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/d661c142-03a1-4de1-b20b-5b43068fe3e4)



### 25. egrep 'Linux.*World' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/15fa5679-2d8d-4e02-b277-ba63b7b90da9)



### 26. egrep l{2} newfile
## OUTPUT
![image](https://github.com/user-attachments/assets/e4e05d37-9e0d-4614-bf5b-adca9f85be26)




### 27. egrep 's{1,2}' newfile
## OUTPUT 
![image](https://github.com/user-attachments/assets/f5f29bab-11c9-4968-a4ce-ecb3d30b0a24)



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


### 28. sed -n -e '3p' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/fd318f84-09c2-4821-be8a-1c8d5dd25844)



### 29. sed -n -e '$p' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/db5d83ba-b7f0-46e9-9e78-c6198abedae6)



### 30. sed  -e 's/Ram/Sita/' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/89f2b6f2-a017-4eab-a31a-e0365dc43890)



### 31. sed  -e '2s/Ram/Sita/' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/f0ca9460-3b8b-4b51-a19f-689436cc7bf5)



### 32. sed  '/tom/s/5000/6000/' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/76235b07-eaee-465b-bba8-08ef28447b4a)



### 33. sed -n -e '1,5p' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/46df2d92-bcda-4a5f-8a08-898626be17cb)




### 34. sed -n -e '2,/Joe/p' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/ab02e15d-3883-4874-8036-be7b6d7b8be3)




### 35. sed -n -e '/tom/,/Joe/p' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/6d6e3458-a51c-46af-b100-3c137ab2c100)



### 36. seq 10 
## OUTPUT
![image](https://github.com/user-attachments/assets/911cb8f0-5f1b-4137-b76f-e09802129fa3)



### 37. seq 10 | sed -n '4,6p'
## OUTPUT
![image](https://github.com/user-attachments/assets/8181e2c7-70ca-4aa0-a107-40df3871bbdb)



### 38. seq 10 | sed -n '2,~4p'
## OUTPUT
![image](https://github.com/user-attachments/assets/30b38f71-03b3-4ce8-8ec1-8b58d3629742)



### 39. seq 3 | sed '2a hello'
## OUTPUT
![image](https://github.com/user-attachments/assets/29759d91-123c-4d9f-894a-9d8401759bf0)



### 40. seq 2 | sed '2i hello'
## OUTPUT
![image](https://github.com/user-attachments/assets/e0bd26a3-cb2f-42d4-b722-bd0fa8c1b621)


### 41. seq 10 | sed '2,9c hello'
## OUTPUT
![image](https://github.com/user-attachments/assets/d7d0b29c-d238-47af-8a8d-7536da82e015)


### 42. sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
![image](https://github.com/user-attachments/assets/b6063a05-8971-4fdd-8302-db9fe0f86e51)



#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 

### 43. sort file21
## OUTPUT
![image](https://github.com/user-attachments/assets/3d80105e-4bf7-441a-abf2-c61d7f0f5970)



cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 

### 44. uniq file22
## OUTPUT
![image](https://github.com/user-attachments/assets/52893b1e-40a3-4280-9bcb-93bafc480488)



## Using tr command
### 45. cat file23 | tr [:lower:] [:upper:]
## OUTPUT
![image](https://github.com/user-attachments/assets/9fdb7a17-fc07-4163-b907-7105607f3fc8)



cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```

### 46. cat urllist.txt | tr -d ' '
## OUTPUT
![image](https://github.com/user-attachments/assets/607c7b65-bb31-4916-80a7-2e0b8f75e3aa)


 
### 47. cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
![image](https://github.com/user-attachments/assets/e0d32da5-3132-4155-83d5-8df5e6692cea)



## Backup commands
tar -cvf backup.tar *
## OUTPUT


mkdir backupdir
 
mv backup.tar backupdir
 
tar -tvf backup.tar
## OUTPUT


tar -xvf backup.tar
## OUTPUT

gzip backup.tar

ls .gz
## OUTPUT
 
gunzip backup.tar.gz
## OUTPUT

 
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

 
ls file1
## OUTPUT

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 
abcd
 
echo $?
 ## OUTPUT


 
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

## OUTPUT


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


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT



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
## OUTPUT 


# RESULT:
The Commands are executed successfully.
