# Win2Linux
summarize some functions and replacement ideas in the process of the translation from win to linux

## function
_splitpath\<br>
copyFile

## direct replacements
#include <unistd.h>
_access(const char * targetDir, 0) -> access(const char * targetDir, 0) 

#include <sys/stat.h>
_mkdir( const char * targetDir) -> mkdir(const char * targetDir, S_IRWXU|S_IRWXG)
