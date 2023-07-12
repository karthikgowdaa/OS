#include<stdio.>
#include<unistd.h>
#include<sys/wait.h>

int main()
{
pid_t pid;
int status;
pid=fork()

if(pid<0){
printf("error:fork()failed.\n);
return 1;
}else if(pid==0)
{
printf("this is the child process with pid:%d\n",getpid());
printf("parent process pid:%d\n",getppid());
execlp("/bin/ls","ls",NULL);

printf("thois should not be printed if exec() is successful:\n");
return 0;
}
else
{
printf("this is the parent process with pid:%d\n",getpid());
printf("child process pid:%d\n",pid);
wait(&status);
printf("child process exited with status:%d\n",status);
return 0;
}
}


