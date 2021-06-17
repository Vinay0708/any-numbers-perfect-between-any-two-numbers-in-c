# any-numbers-perfect-between-any-two-numbers-in-c
#include<stdio.h>
int main()
{   int n,i,sum,a,b;
    printf("Enter two numbers: between find perfect number:");
    scanf("%d %d",&a,&b);
    for(n=a;n<=b;n++)
    {  
        sum=0;
       for(i=1;i<=n-1;i++)
       {
       if(n%i==0)
       sum=sum+i;
       }
    if(sum==n)
    printf("the number %d is perfect \n",n);
    }    
return 0;
}
