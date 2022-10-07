#include<stdio.h>
#include<conio.h>
#include<string.h>
int main()
{
	int nf=0,i=0,j=0,ch;
	char mdname[20],fname[10][10],name[10];
	printf("enter the directory name :");
	scanf("%s",&mdname);
	printf("enter n umber of files :");
	scanf("%d",&nf);
	do
	{
		printf("enter file name to be creted :");
		scanf("%s",name);
		for(i=0;i<nf;i++)
		{
			if(!strcmp(name,fname[i]));
			break;
			}
			if(i==nf)
			{
				strcpy(fname[j++],name);
				nf++;
			}
			else
			printf("there is already a directory %s\n",name);
			printf("do you want to enter another file(yes-1 or no-0):");
			scanf("%d",&ch);
		}while(ch==1);
		printf("directory name is :%s\n",mdname);
		printf("files name are");
		for(i=0;i<j;i++)
		{
			printf("\n%s",fname[i]);
			}
			getch();
	}
