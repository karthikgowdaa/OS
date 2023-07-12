#include<stdio.h>
#include<string.h>
main()
{
Int i=0,pno[10],bt[10],n,wt[10],temp=0,j,tt[10];
float sum,at;
printf("\n Enter the no of process ");
scanf(" %d",&n);
printf("\n Enter the burst time of each process");
for(i=0;i<n;i++)
{
printf("\n p%d",i);
scanf("%d",&bt[i]);
}
for(i=0;i<n-1;i++)
{
for(j=i+1;j<n;j++)
{
if(bt[i]>bt[j])
{
temp=bt[i];
bt[i]=bt[j];
bt[j]=temp;
temp=pno[i];
pno[i]=pno[j];
pno[j]=temp;
}
}
}
wt[0]=0;
for(i=1;i<n;i++)
printf("\nAverage Waiting time:%f", (float)totwt/n);
printf("\nAverage Turn Around Time:%f", (float)tottat/n);
}
