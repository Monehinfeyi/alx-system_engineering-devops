THIS DIRECTORY CONTAINS IMPORTANT COMMANDS AND SCRIPTS

### TASK:0x03. Shell, init files, variables and expansions

0. <o> - This script creates an alias

#!/bin/bash
alias ls='rm *'

1. Hello you  - This script prints hello user, where user is the current Linux user.

#!/bin/bash
echo hello $USER

2. The path to success is to take massive, determined action - Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program



3. If the path be beautiful, let us not ask where it leads - The script counts the number of directories in the PATH

#!/bin/bash
echo $(printf $PATH | tr ":" "\n" | wc -w)

4. Global variables - The script lists environment variables.

#!/bin/bash
printenv


5. Local variables - This script lists all local variables and environment variables, and functions.

#!/bin/bash
set | less
