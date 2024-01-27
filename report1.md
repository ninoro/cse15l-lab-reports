__Lab Report 1 - Remote Access and FileSystem (Week 1)__
-------------

<br>- Using Command `cd`<br>
  1) No arguments
  <br> _Working Directory_: home <br>
     The `cd` command changes the current directory to the one mentioned as the argument. Since there is no argument, `cd` remains in the working directory which is home here.
      <br> _Error_: No Errors <br>
     
  ![Image](img11.png)

  <br> _Working Directory_: messages <br>
      The 'cd' command changes the current directory to home.
      <br> _Error_: No Errors <br>

  ![Image](img11.png)

  2) Command with a path to a directory
  <br> _Working Directory_: home <br>
       The `cd` command changes the current directory to lecture1.
     <br> _Error_: No Errors <br>

  ![Image](img1.png)
     
  3) Command with a path to a file
  <br> _Working Directory_: lecture1 <br>
       The `cd` command changes the current directory to messages.
     <br> _Error_: No Errors <br>

  ![Image](img1.png)

<br>- Using Command `ls`<br>
  1) No arguments
  <br> _Working Directory_: home <br>
    The `ls` command displays the files or folders in the path entered as the argument. Since there is no argument, the folders in the current directory are displayed.
     <br> _Error_: No Errors <br>

  ![Image](img7.png)
     
  2) Command with a path to a directory
  <br> _Working Directory_: home <br>
      The `ls` command displays the folders in the lecture1 path.
     <br> _Error_: No Errors <br>

   ![Image](img7.png)
     
   3) Command with a path to a file
   <br> _Working Directory_: home <br>
     _Error_: The `ls` command cannot display the folders or files present in messages without first moving to the lecture1 directory.

  ![Image](img7.png)
      
  <br> _Working Directory_: lecture1 <br>
    The `ls` command now displays the files present in messages.
    <br> _Error_: No Errors <br>

  ![Image](img7.png)

<br>- Using Command `cat`<br>
  1) No arguments
  <br> _Working Directory_: home <br>
     The `cat` command prints out the contents of the file. Since there is no argument, the `cat` command will display the content of the text entered as standard input.
     <br> _Error_: No Errors <br>

  ![Image](img8.png)
     
  2) Command with a path to a directory
  <br> _Working Directory_: home <br>
      _Error_: The `cat` command cannot read the contents the lecture1 directory mentioned as the argument, giving the output that the argument mentioned is a directory.

  ![Image](img8.png)
     
  <br> _Working Directory_: home <br>
      _Error_: The `cat` command is not run in the lecture1 directory, so the messages folder is not recognized.

  ![Image](img8.png)
     
  3) Command with a path to a file
  <br> _Working Directory_: home <br>
    The `cd` command changes the directory to lecture1
    <br> _Working Directory_: lecture1 <br>
    _Error_: messages is a directory like the output states, not a file.

   ![Image](img40.png)
     
   <br> _Working Directory_: messages <br>
     The `cat` command reads the content of the `en-us.txt` file and prints out the output. (Misspelled `txt` as `text` the first time, eeps)
     <br> _Error_: No Errors <br>

   ![Image](img41.png)

     

     
  
  

     


