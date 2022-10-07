![Screenshot (54)](https://user-images.githubusercontent.com/112555562/194502434-df97114d-4a81-4adc-bdfe-0180cba010b5.png)
# operting-system

![image](https://user-images.githubusercontent.com/112555562/194502651-63a4b218-e7b3-44f4-a5b0-2ddf67cc2399.png)
#include<stdio.h>
#include<stdlib.h>
#include<sys/types.h>
#include<unistd.h>
int main(void)
{
	pid_t pid=fork();
	if(pid==0)
	{
		printf("Child = PPID: %d PID: %d\n",getppid());
		exit(EXIT_SUCCESS);
	}
	else if(pid>0)
	{
		printf("Parent = PID: %d\n",getpid());
		printf("Waiting for child process to finish.\n");
		wait(NULL);
		printf("Child process finished.\n");
	}
}
