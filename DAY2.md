QN:C program to check the validity of a string.
CONDITION: * > #   positive integer
	     # > *    negative integer
	     *==#    0

#include<stdio.h>
#include<string.h>
int main()
{
char a[10];
int count1=0,count2=0,count3=0,count4=0,i;
printf("enter the string:");
scanf("%s",a);
printf("%s",a);
for(i=0;i<strlen(a);i++)
{
if(a[i]=='#')
{
count1++;
}

if(a[i]=='*')
{
count2++;
}
}
if(count1>count2)
{
count3=count1-count2;
printf("\n%d",count3);
}
else if(count2>count1)
{
count4=count1-count2;
printf("\n%d",count4);
}
else
{
printf("\n0");
}
return 0;
}


QN:Create a 1D array find the sum of the number and check whether it  is prime or not.

#include<stdio.h>
int main()
{
int a[10],n,i,sum=0,count=0;
printf("Enter the limit:");
scanf("%d",&n);
printf("Enter the elements:\n");
for(i=0;i<n;i++)
scanf("%d",&a[i]);
for(i=0;i<n;i++)
{
sum=sum+a[i];
}
printf("Sum=%d\n",sum);
for(i=1;i<sum/2;i++)
{

    if(sum%2==0)

    count++;
}
if(count==0)
printf("%d  is a prime number",sum);
else
    printf("%d is not a prime number",sum);

return 0;
}

QN: Write a C program to create a 1D array and find the reverse of the array and repalce '0' with '$'

#include<stdio.h>
int main()
{
    char r='$';
int n,i,temp,j;
int a[10];
printf("Enter the size of the array:");
scanf("%d",&n);
printf("Enter the elements:");
for(i=0;i<n;i++)
{
    scanf("%d",&a[i]);
}
for(i=0,j=n-1;i<j;i++,j--)
{
    temp=a[i];
    a[i]=a[j];
    a[j]=temp;
}
printf("Reversed array\n");
for(i=0;i<n;i++)
{
    printf("%d\t",a[i]);
}
    for(i=0;i<n;i++)
{
if(a[i]==0)
{
a[i]=r;
}
}
printf("\nReplaced array\n");
for(i=0;i<n;i++)
{
    printf("%d\t",a[i]);
}

return 0;
}

QN:  write a C program to find sum of 2 numbers using pointer.

#include<stdio.h>
int main()
{
int a=20,b=30,sum;
int *p1,*p2;
p1=&a;
p2=&b;
sum=*p1+*p2;
printf("%d",sum);
return 0;


QN:write a C program to swap two numbers using  pointers.

#include<stdio.h>
int main()
{
int a=20,b=30;
int *p1,*p2,temp;
printf("value of a=%d",a);
printf("\nvalue of b=%d",b);
temp=*p1;
*p1=*p2;
*p2=temp;
printf("value of a=%d",*p1);
printf("Value of b=%d",*p2);
return 0;
}
QN:Write a C porgram to print a 2D array.
#include<stdio.h>
int main()
{

int n,m,i,j;
int a[10][10];
printf("Enter the no.of rows:");
scanf("%d",&n);
printf("Enter the no.of columns:");
scanf("%d",&m);
printf("Enter the elements:");
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
scanf("%d",&a[i][j]);
}
}
printf("Matrix\n");
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
printf("%d\t",a[i][j]);
}
printf("\n");
}
return 0;
}


QN:Write a c program to find the diagonal,upper diagonal and lower diagonal of a 2D array.

#include<stdio.h>
int main()
{

int n,m,i,j;
int a[10][10];
printf("Enter the no.of rows:");
scanf("%d",&n);
printf("Enter the no.of columns:");
scanf("%d",&m);
printf("Enter the elements:");
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
scanf("%d",&a[i][j]);
}
}
printf("Matrix\n");
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
printf("%d\t",a[i][j]);
}
printf("\n");
}

printf("Diagonal elements:\n");
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
if(i==j)
{
printf("%d\t",a[i][j]);
}
}
}
printf("\nUpper Diagonal elements:\n");
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
if(i<j)
{
printf("%d\t",a[i][j]);
}
}
}
printf("\nLower Diagonal elements:\n");
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
if(i>j)
{
printf("%d\t",a[i][j]);
}
}
}
return 0;
}
