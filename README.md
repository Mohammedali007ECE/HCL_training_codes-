# HCL_training_C_codes
learning and studing of HCL concepts with respect to concepts , development, and debugging.
# EXERCISE
~~~
1.Reading_output_from_an_external_program

#include<unistd.h>
#include<stdlib.h>
#include<stdio.h>
#include<string.h>
int main() {
FILE *read_fp;
char buffer[BUFSIZ+1];
int chars_read;
memset(buffer,'\0',size of(buffer));
read fp = popen("uname -a","r");
if(read_fp!=NULL){
chars_read=fread(buffer,size of (char) , BUFFSIZ, read fp);
if(chars_read>0) {
printf("output was: -\n%s\n",buffer);
}
pclose(read_fp);
exit(EXIT_SUCCESS);
}
exit(EXIT_FAILURE);
}
~~~
~~~
2.Basic_Syntax_template_to_write (popen)

#include<stdio.h>
#include<stdlib.h>
int main() {
FILE *fp;
char buffer [1024];
fp=fopen ("your_command_here","r");
if (fp==NULL) {
perror ("popen failed");
exit (EXIT_FAILURE);
}
while (fgets(buffer,size_of(buffer,fp)!=NULL){
printf("output was : -\n%s\n",buffer);
}
pclose(read_fp);
exit(EXIT_SUCCESS);
}
exit(EXIT_FAILURE);
}
~~~
~~~
3.Basic_Syntax_for_Reading_the_output

#include<stdio.h>
#include<unistd.h>
int main()
{
int fd[2];
char buffer [100];
pipe (fd);
write (fd[1],"Hello",5);
read (fd[0],buffer, 5);
buffer [5]='\0';
printf("output:%s\n",buffer);
return 0;
}
~~~
