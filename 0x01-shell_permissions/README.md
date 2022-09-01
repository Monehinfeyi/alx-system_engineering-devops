TASK=[0x01. Shell, permissions]
THIS DIRECTORY CONTAINS SOME COMMANDS WHICH ARE USED TO SET PERMISSION IN LINUX AND THEY ARE TO RUN IN UBUNTU 20.04 LTS AND ALSO CONTAINS SCRIPTS

LINUX COMMANDS TO SET PERMISSION

chmod - modify file access rights
su - temporarily become the superuser
sudo - temporarily become the superuser
chgrp - change a file's group ownership
chown change file ownership

            TASKS

[0. My name is Betty]   This create a script that changes user ID to betty.

#!/bin/bash
su betty

[1. Who am I]   This script prints the effective username of the current user.

#!/bin/bash
whoami

[2. Groups]  This script prints all the groups the current user is part of.

#!/bin/bash
groups

[3. New owner] This script changes the owner of the file hello to the user betty.

#!/bin/bash
chown betty hello

[4. Empty!] -This script creates an empty file called "hello"

#!/bin/bash
touch hello

[5. Execute] -This script adds execute permission to the owner of the file "hello".The file hello will be in the working directory.

#!/bin/bash
chmod u+x hello

[6. Multiple permissions] -This script adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

#!/bin/bash
chmod u+x,g+x,o+r hello

[7. Everybody!] -This script adds execution permission to the owner, the group owner and the other users, to the file "hello".

#!/bin/bash
chmod ugo+x hello

[8. James Bond] -This script sets the permission to the file "hello" as follows:
-Owner: no permission at all
-Group: no permission at all
-Other users: all the permissions

#!/bin/bash
chmod 007 hello

[9. John Doe] - This script sets the mode of the file "hello" in the working directory.

#!/bin/bash
chmod 753 hello

[10. Look in the mirror] - This script sets the mode of the file "hello" the same as "olleh"’s mode.The file "hello" and "olleh" will be in the working directory.

#!/bin/bash
chmod --reference olleh hello

[11. Directories] - This script adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files will not be changed.

#!/bin/bash
chmod -R a+X ./

[12. More directories] -This script creates a directory called "my_dir" with permissions 751 in the working directory.

#!/bin/bash
mkdir -m 751 my_dir

[13. Change group] -This script changes the group owner to "school" for the file "hello".The file "hello" will be in the working directory

#!/bin/bash
chgrp school hello






