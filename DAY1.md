DAY-1

QN: C program to  get 3 sides of triangle as input and find out whether a triangle can be framed or not.

#include<stdio.h>
int main()
{
    int side1,side2,side3;
printf("Enter the sides:\n");
scanf("%d%d%d",&side1,&side2,&side3);
if(side1+side2>side3 || side2+side3>side1 || side1+side3>side2)
{
printf("The triangle can be framed\n");
}
else
{
printf("The triangle cannot be framed\n");
}
return 0;
}

QN:Sam is having 75 candies  all of which half he gave to his close friend Angel. Now Angel loves Sam alot so she gave half back to Sam. How many candies Sam have?

#include<stdio.h>
int main()
{
    float x,y,z;
    x=75/2;
    y=x/2;
    z=x+y;
    printf("Sam has %f",z);
    return 0;
}
