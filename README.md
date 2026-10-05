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
