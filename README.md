# Configure-Yum
The yum command in Linux is a package manager used primarily in Red Hat-based distributions, such as Red Hat Enterprise Linux (RHEL), CentOS, and Fedora. Its primary purpose is to manage the installation, updating, and removal of software packages on a Linux system. We do also have rpm command for the same purpose,but there are some softwares who are dependednt on some other softwares,this is known as dependency.rpm command is not able to solve dependency on its own which generates the need of yum command.

# Load the ISO File and copy path

![WhatsApp Image 2023-08-23 at 2 12 04 AM](https://github.com/neelay-16/Configure-Yum/assets/135517502/b952fe6a-84a4-49d8-b96e-544e21d89005)


When configuring yum on a Red Hat-based Linux distribution like CentOS or RHEL (Red Hat Enterprise Linux), you typically create repository configuration files, including local.repo or custom .repo files, to specify where yum should look for packages. These repository files allow you to define the source repositories for software packages that yum can install and manage.The AppStream and BaseOS repositories are important components of these distributions:
1. BaseOS: The BaseOS repository contains the core packages and libraries that form the foundation of the operating system. These packages provide essential system functionality and typically don't change very frequently. Examples of packages in the BaseOS repository include the kernel, system libraries, and basic command-line utilities.

2. AppStream: The AppStream repository contains a wide range of software packages that can be installed on top of the base operating system. This repository includes applications, development tools, libraries, and other software that extends the functionality of the system. The packages in AppStream are typically updated more frequently than those in BaseOS.

![WhatsApp Image 2023-08-29 at 8 48 05 PM](https://github.com/neelay-16/Configure-Yum/assets/135517502/698d49c4-d8ec-4394-a622-7b4370170ea1)

# Check that yum is configured

To check whether the yum command is configured and available on your Linux system, there are many ways such as:
1. You can typically find this in the applications menu or by using a keyboard shortcut like 'Ctrl+Alt+T'.
2. You can check if yum is installed on your system by running the following command:

   ![image](https://github.com/neelay-16/Configure-Yum/assets/135517502/fbacbef6-2787-4ae2-ade5-91e6f0bbff22)

This command will display the version information of yum if it's installed. 
3.  You can also test yum by running a simple command. For example, you can try to list the installed packages using the following command:

![image](https://github.com/neelay-16/Configure-Yum/assets/135517502/e4914434-3c5a-4ddb-b768-f94303217b6b)

If yum is configured correctly, it will list the installed packages on your system.
4. yum configuration files are typically located in the '/etc/yum/ directory'. You can check if this directory exists and contains configuration files like 'yum.conf' or any .repo files. Here's how you can list the contents of the /etc/yum/ directory: 

![image](https://github.com/neelay-16/Configure-Yum/assets/135517502/d8ad3a2c-427d-4504-bcc9-75145f072d9d)

If you see configuration files in this directory, it indicates that yum is configured on your system.
5. The yum binaries should be located in the /usr/bin/ directory. You can check for the presence of these binaries using the ls command:

![image](https://github.com/neelay-16/Configure-Yum/assets/135517502/bfa03a50-c757-487c-a1ca-09e6aa639962)

6. Also,you can try installing any software through yum command to check whether 'yum' command is properly configured or not.
![WhatsApp Image 2023-08-23 at 2 12 54 AM](https://github.com/neelay-16/Configure-Yum/assets/135517502/e3a742cb-8766-456d-8eca-31e383457faf)

![WhatsApp Image 2023-08-23 at 2 13 42 AM](https://github.com/neelay-16/Configure-Yum/assets/135517502/e71356b7-3f58-4a66-a4b1-32c4d4a62e49)


'dnf' command is also another alternative for 'yum' command.

