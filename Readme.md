### Build executables

- make

### Remove executables

- make clean

### Update PATH to point to your custom shell counterpart

- export PATH=$(pwd):$PATH

### Utilities supported

#### cat

### Example Usage

- cat zen.txt
- cat -o zen1.txt zen.txt
- cat -a zen1.txt zen.txt
- cat -o zen1.txt zen.txt test.txt
- cat -a zen1.txt zen.txt test.txt
- cat -n zen.txt

P.S: The order of the flags for the cat utility matters since that's how getopts parses. In later versions,
     adding a customized parsing logic could help resolve it.

#### find

### Example Usage

- find /path
- find /path -name <file_name>
- find /path -iname <file_name>
- find /path -type f
- find /path -type d
- find /path -type f -name <file_name>
- find /path -type d -name <dir_name>
- find /path -size +100M
- find /path -user <user_name> -group <group_name>
- find /path -perm <r,w,x,rw,rx>
