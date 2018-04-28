#include<stdio.h>
#include<string.h>
#include<stdlib.h>
int main()
{
int noOfProcess, root, timeQuantum, totalTime=0, averageTime;
int studentArray[100];
char sirName[20];
printf("\nAre you HR?Enter 1 if yes");
scanf("%d", &root);
if(root==1)
{
printf("\nEnter Your Name, Sir");
scanf("%s", &sirName);
printf("\nWelcome %s", sirName);
printf("\nYour time is from 10 to 12 AM");
printf("\n-------------------------------------------");
printf("\nEnter no of students:");
scanf("%d",&noOfProcess);
printf("\nEnter the time Quantum:");
scanf("%d", &timeQuantum);
for(int i=0; i<noOfProcess; i++)
{
studentArray[i] = i+1;
}
for(int i=120, j=0; i>0, j<noOfProcess; i=i-timeQuantum, j++)
{
printf("\nThe doubt query handled %d", i);
printf("\nthe student is:%d",studentArray[j]);
totalTime = totalTime + timeQuantum;

}
averageTime = (totalTime/noOfProcess);
printf("----------------------------------------------------------------");
printf("\nThe total Time handled by the person is : %d", totalTime);
printf("\nThe average time Query is %d", averageTime);
}
else
{
printf("\nSorry the server is down");
printf("\nTry again later");
}
}
