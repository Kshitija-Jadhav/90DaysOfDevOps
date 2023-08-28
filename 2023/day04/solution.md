- Explain in your own words and examples, what is Shell Scripting for DevOps.

Shell scripting in terms of DevOps is using scripts written in a shell language (like Bash on Linux with .sh extension) to automate tasks in the software development and operations processes.
It's a way to bridge the gap between software development (Dev) and IT operations (Ops) by automating tasks that help in deploying, managing, and monitoring software systems.

Some examples of how shell scripting is used in DevOps:

1. Continuous Integration and Testing: In the DevOps pipeline, shell scripts can be used to automate the build and testing of software applications. This helps ensure that code changes don't break the existing functionality.
2. Release Management: When it's time to release a new version of the software, shell scripts can automate tasks like updating documentation, tagging the version in version control, and notifying stakeholders.
3. Infrastructure Provisioning: DevOps frequently involves creating and managing infrastructure as code. Shell scripts can be used to provision virtual machines, containers, or cloud resources like instances and storage.

- What is `#!/bin/bash?` can we write `#!/bin/sh` as well?

The #!/bin/bash line, often referred to as the "shebang," is a special instruction used at the beginning of shell scripts. It tells the system which interpreter to use for executing the script.
#!/bin/bash specifies that the script should be interpreted and executed using the Bash shell. Bash (short for "Bourne Again Shell") is a popular and powerful command-line shell and scripting language.
You can use #!/bin/sh in the shebang line to indicate that the script should be interpreted and executed using the system's default shell, which is usually a POSIX-compliant shell.

The difference between #!/bin/bash and #!/bin/sh lies in the specific shell interpreter being used to execute the script.
#!/bin/bash: Uses the Bash shell for script execution. Provides Bash-specific features.
#!/bin/sh: Uses the default shell for script execution, which can vary between systems.
If you require Bash-specific features or scripting capabilities, use #!/bin/bash. If you want your script to be more portable and work on a wider range of systems, you might opt for #!/bin/sh.

- Write a Shell Script which prints `I will complete #90DaysOofDevOps challenge`
1. First, create a directory dedicated only to the scripts using the below command:
mkdir scripts

2. Create a script using the command "nano devops1.sh"

#!/bin/bash
echo "I will complete #90DaysOfDevOps challenge"

3. Run the script using the command bash devops1.sh

- Write a Shell Script to take user input, input from arguments and print the variables.

1. Create a script using the command "nano readinput.sh"
#!/bin/bash

echo "Read input from user"
echo "Enter your name:"
read name
echo "Name: " $name

2. Run the script using the command bash devops1.sh

- Write an Example of If else in Shell Scripting by comparing 2 numbers

1. Create a script using the command "nano compare_2_nos.sh"

#!/bin/bash
echo "Enter the first number:"
read num1
echo "Enter the second number:"
read num2
if [ $num1 -gt $num2 ]; then
    echo "$num1 is greater than $num2"
elif [ $num1 -lt $num2 ]; then
    echo "$num1 is less than $num2"
else
    echo "$num1 is equal to $num2"
fi

2. Run the script using the command bash compare_2_nos.sh


