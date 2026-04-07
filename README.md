Exercise 00: Z

create a file name "z" with the content of "Z"
>> echo "Z" > z

Exercise 01: testShell00

create a file name "testShell00", with the permission of 
r = 4, w = 2, x = 1, --- = 0. Octal representation
(Read [r--]) 4, (Read + Execute [r-x]) 4+1, and (read Execute [r-x]) 4+1 for (owner, group, others)
-r--r-xr-x
>> touch testShell00  #This create files 
>> chmod 455 testShell00  #This create permission for testSHell00

Exercise 02: Oh yeah, mooore..

drwx--xr-x  :: "d" is directory, to acheive that create a directory
create files that has no "d" on it
File permission "rwd" can reference from Exercise01

-r-----r-- 2 XX XX 1 Jun 1 23:44 test3  :: the value 2 is a Link count, can be only change by adding/removing link
ln test3 <Desire_name>  #This will change the Link count for "test3"
XX XX 1  :: the value 1 represent the bytes long, size will become larger by adding long context
>> echo "Hello" > test1

lrwxrwxrwx 1 XX XX 5 Jun 1 22:20 test6 -> test0  :: Create a shortcut for test6
>> ln -s test0 test6  #This will add a "l" in front
