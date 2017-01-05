# unleash
A lean shell program developed as part of IIT's CS551 course

REQUIREMENTS :

1) Shell shall be invoked from the Ash shell provided with Minix.

2) Shell shall first execute a PROFILE file which defines a HOME variable. 
   Once the PROFILE file is executed, we will be in the HOME directory. 
   This HOME variable does not replace the one from the Ash shell. 
   
3) Prompt shall display the current directory name.

4) In a command line of the shell we should be able to exercise any executable programs 
   including the utilities provided in /bin and /usr/bin.
   
5) Shell shall support the execution of a list of commands in the following format: 

		curdir command1, command2, (command3)
		
   The precedence of the commands are from left to right but parenthesized commands supersedes that order. 
   In the example, command3 has highest precedence, followed by command1 then command2. 
   
   Parenthesis may be nested. 
   Two or more commands within the same pairs of parenthesis separated by a “,” are intended to be executed in parallel. 

6) Shell shall support an alias command. It will allow the user to type the name of an alias and have 
   the shell expand it internally to the string that the name replaces, and if the string is a valid command, executes it. 
   Once an alias is defined, it becomes persistent. 
   
   For example, the user may first define: 

		Alias listcontent=“ls”
		And later type $ listcontent –l
		Then the command ls –l will be executed.

   Should not use Ash shell environmental variables to implement this.
   
7) Shell can only be terminated by exit and ctrl-c. 
   If it is the latter, shell shall ask “Are you sure?” and exit after confirmation.
   

Project hosted privately at https://bitbucket.org/sashankbv/unleash
