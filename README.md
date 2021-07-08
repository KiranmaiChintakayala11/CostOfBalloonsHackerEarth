#include <stdio.h>
 
int main()
{
int num,p,c[2];
scanf("%d", &num); 
for(int k=0;k<num;k++)
{ 
int green,purple;
scanf("%d %d",&green,&purple);
 
scanf("%d",&p);
int person[p][2];
int cost1=0,cost2=0;
for(int i=0;i<p;i++)
{
for(int j=0;j<2;j++)
{
scanf("%d",&person[i][j]);
if(person[i][j]==1)
{
if(j==0)
cost1=cost1+green;
else
cost1=cost1+purple;
}
if(person[i][j]==1)
{
if(j==0)
cost2=cost2+purple;
else
cost2=cost2+green;
}
} 
 
}
if(cost1>cost2)
printf("%d\n",cost2);
else
printf("%d\n",cost1);
}
 
}
