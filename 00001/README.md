# learnjavascript
Project Assignment 1: Beginner

1. Write the command that will allow you to navigate to two directories above your current directory. Study
   these examples: 
   <br>Current directory or path:
   <br>Ryan@RyansLaptop ~/Coursework/Fall 2015/BIOL13/
   <br>Steve@FamilyComputer ~/My Documents/Book Library/Francine Jay/The Joy of Less/
   <br>The directory or path that is two directories above the “current” one shown above:
   <br>Ryan@RyansLaptop ~/Coursework/
   <br>Steve@FamilyComputer ~/My Documents/Book Library/
   <br>Ans: cd ../.. 

2. Write the command and flag that will list the files and directories inside of your current directory.
   <br>Ryan@RyansLaptop ~/Coursework/Fall 2015/
   <br>Steve@FamilyComputer ~/My Documents/
   <br>Example output:
   <br>ACCT20 BIOL13 BIOL20 CSCI2 schedule.txt
   <br>Book Library Pictures Printing Videos index.html test.css
   <br>Ans: ls

3. Write the command and flag that will list all of the files and directories in your current directory in longformat.
   <br>Current directory or path:Ryan@RyansLaptop ~/Coursework/Fall 2015/ <br>Example output: 
   <br>total 1
   <br>drwxr-xr-x 1 Ryan Ryan 0 Aug 14 18:36 ACCT20/
   <br>drwxr-xr-x 1 Ryan Ryan 0 Aug 14 13:52 BIOL13/
   <br>drwxr-xr-x 1 Ryan Ryan 0 Aug 14 18:22 BIOL20/
   <br>drwxr-xr-x 1 Ryan Ryan 0 Aug 14 12:11 CSCI2/
   <br>-rw-r--r-- 1 Ryan Ryan 5 Aug 11 13:37 schedule.txt
   <br>Ans:ls -l 
4. Write the command and flag that will list all of the files and directories in your current
   directory, including hidden files.
   <br> Current directory or path:
   <br> Ryan@RyansLaptop ~/Coursework/Fall 2015/ <br> Example Output
   <br> ./ ../ .magic ACCT20/ BIOL13/ BIOL20/ CSCI2/ schedule.txt
   <br> Ans: ls -a

5. Write the command that will create a folder in your current working directory and name
   it clean_code_examples .
   <br> Current working directory’s ls:
   <br> ACCT20 BIOL13 BIOL20 CSCI2 schedule.txt
   <br> Current working directory after the ls command was run:
   <br> ACCT20 BIOL13 BIOL20 clean_code_examples CSCI2 schedule.txt
   <br> Ans: mkdir clean_code_examples

6. Write the command to create a new file. Give the file a name and use the .txt extension.
   <br> Current working directory’s after the ls command was run on it:
   <br> dog photos family photos cooking recipes
   <br> Resulting Current Working Directory’s ls
   <br> dog photos family photos cooking recipes anynamethatidlike.txt
   <br> Ans: touch mytextfile.txt

7. Write the command that will output the contents of the file socks to buy.txt , located in your current
   working directory, to the terminal. Assume that either socks to buy.txt already exists, or create it
   yourself.
   <br> Example output (contents of socks to buy.txt)
   <br> I should wait to buy socks until next Fall.
   <br> Ans: cat 'socks to buy.txt'

8. Write the command to display your Present Working Directory.
   <br> Example GitBash Output
   <br> /c/Users/Ricardo/dota2/
   <br> Ans: pwd

9. Write the command to output the current user to the terminal. Thecurrent user is generally the account that
   is logged into the operating system and currently using the terminal.
   <br> Example GitBash output:
   <br> Richardo
   <br> Ans: id -nu or whoami

10. Write the command to list the files and folders of the folder two above your current directory. For example,
    if you are in C:/Users/John Wayne/My Documents/Tax Forms/ , display all files and folders within the
    <br> directory C:/Users/John Wayne/ .
    <br> Current directory or path:
    <br> Ryan@RyansLaptop ~/Coursework/Fall 2015/BIOL13/
    <br> Example GitBash output:
    <br> /Coursework:
    <br> Fall 2016/ Spring 2015/ Spring 2016/
    <br> Ans:ls ../..

11. Write the command to create the file list of best cat pictures.html .
    <br> Example current directory:
    <br> images javascript css vectors index.htm gallery.htm contact.htm
    <br> Example output:
    <br> images javascript css vectors contact.htm index.htm gallery.htm list of best cat picture
         s.html
    <br> Ans:touch "list of best cat pictures.html"

12. Write the command that will change your current directory to C:/Users/Default User/My Documents .
    Note: the directory C:/Users/Default User/My Documents may not exist on your computer; if that is the
    case, you’ll see the error bash: cd: C:/Users/Default User/My Documents: No such file or
    directory
    <br>Initial working directory:
    <br>Ryan@RyansLaptop ~/Coursework/Fall 2015/BIOL13/
    <br>Directory after executing command:
    <br>Ryan@RyansLaptop /c/Users/Default User/My Documents
    <br>Ans:cd "/C/Users/Default User/My Documents"

13. Write the command that will ping the ip address 8.8.8.8 .
    <br> Example output:
    <br> Reply from 8.8.8.8: bytes=32 time=23ms TTL=55
    <br> Reply from 8.8.8.8: bytes=32 time=16ms TTL=55
    <br> Reply from 8.8.8.8: bytes=32 time=18ms TTL=55
    <br> Reply from 8.8.8.8: bytes=32 time=29ms TTL=55
    <br> Ping statistics for 8.8.8.8:
    <br> Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
    <br> Approximate round trip times in milli-seconds:
    <br> Minimum = 16ms, Maximum = 29ms, Average = 21ms
    <br> Ans: ping 8.8.8.8

14. Ans:cd $home
15. Ans:echo "My name is Patel"
16. Ans:cat "tylers favorite songs.txt" "sarahs favorite songs.txt"
17. Ans:help echo > "echo_options.txt" | cat echo_options.txt
18. vi flag 
    <br>CNT=0
    <br>re='^-?[0-9]+$'
    <br>if ! [[ $1 =~ $re ]];
    <br>then
 	<br>echo "error:Not a number. Give +ve number"
    <br>else
	<br>if [ "$1" -lt 1 ];
	  <br>then
   		<br>echo "Give +ve number"
	<br>else
      <br>  	while [ $CNT -lt "$1" ];
        	<br>do
        	<br>ping 127.0.0.1
        	<br>let CNT+=1
        	<br>done
	<br>fi
    <br>fi
    <br>./flag 2
19. cat *.md
20. rm yesterday_todo_list.md

