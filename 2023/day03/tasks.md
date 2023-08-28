Day 3 Task: Basic Linux Commands

Task: What is the linux command to

1. To view what's written in a file.
cat file_name.txt is used to view the contents of the file mentioned.

2. To change the access permissions of files.
In linux, you can change the permissions granted to file using 'chmod' command. The syntax is 'chmod permissions file_name'. The permissions is a 3 digit octal code. There are 3 permissions read (r), write(w) and execute(x) denoted by 4,2,1 bits respectively. There are 3 user permission owner(u), group(g) and other(o).

3. To grant permissions there are 2 ways:
a. Numeric method
To calculate the octal value for each permission combination, you sum the values of the permissions you want to grant.
Syntax:
chmod 761 file_name assigns 761 permission to the file
7 (r+w+x): owner permissions
6 (r+w): group permissions
1 (x): other permissions
b. Symbolic method
In symbolic method we use owner(u), group(g) and other(o) code.
for example. chmod u+x file_name - here we are adding execute permission to owner.

4. To check which commands you have run till now.
'history' command is used to check the commands

5. To remove a directory/ Folder.
To remove file:
rm file_name - this command is used to remove the file mentioned.
To remove directory:
rmdir directory_name - Removes an empty directory
rm -r directory_name - Removes directory and it's contents with recursive option.

6. To create a fruits.txt file and to view the content.
Create a file:
touch fruits.txt - this command will create a new text file with name fruits
Edit the file:
nano fruits.txt - using this command the file can be edited in a nano editor. you can add content to your file and edit it.
View the contents of the file:
cat fruits.txt

7. Add content in devops.txt (One in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava.
Create a file:
touch devops.txt - This command will create a new text file with name devops.
Edit the file:
nano devops.txt - using this command the file can be edited in a nano editor. you can add content to your file and edit it.
Add content:
Inside the nano editor, add each item on a separate line, as requested.
View the contents of the file:
cat devops.txt

8. To Show only the top three fruits from the file.
we use head command for this.
The head command allows you to display the beginning portion of a file.
head -n 3 devops.txt
head is the command to display the beginning of a file.
-n 3 specifies that you want to display the first 3 lines.
devops.txt is the name of the file you want to display the content from.

9. To Show only the bottom three fruits from the file.
we use head command for this.
The tailcommand allows you to display the beginning portion of a file.
tail -n 3 devops.txt
tail is the command to display the beginning of a file.
-n 3 specifies that you want to display the first 3 lines.
devops.txt is the name of the file you want to display the content from.

10. To create another file Colors.txt and to view the content.
Create a file:
touch Colors.txt - this command will create a new text file with name Colors
View the contents of the file:
cat Colors.txt

11. Add content in Colors.txt (One in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey.
nano Colors.txt

12. To find the difference between devops.txt and Colors.txt file.
you can use the 'diff' command with the file names in whcih the difference needs to be found.
diff devops.txt Colors.txt











Reference: https://www.linkedin.com/pulse/linux-commands-devops-used-day-to-day-activit-chetan-/

[← Previous Day](../day02/tasks.md) | [Next Day →](../day04/tasks.md)
