# Simple Calculator

#include<stdio.h>
int Add(int a,int b);
int Subtract(int a,int b);
int Multiplication(int a,int b);
int Divide(int a,int b);
int main()
{
    int x;
    printf("Simple Calculator\n");
    printf("Choose an Option:\n");
    printf("1) Add\n");
    printf("2) Subtract\n");
    printf("3) Multiplication\n");
    printf("4) Division\n");
    printf("Enter Your Choice:");
    scanf("%d",&x);
    
    if (x==1)
    {
        int y,c;
        printf("Addition\n");
        printf("Enter 1st N.o:");
        scanf("%d",&y);
        printf("Enter 2nd N.o:");
        scanf("%d",&c);
        int res;
        res=Add(y,c);
        printf("%d+%d=%d",y,c,res);
        
    }
    else if(x==2)
    {
        int y,c;
        printf("Subtraction\n");
        printf("Enter 1st N.o:");
        scanf("%d",&y);
        printf("Enter 2nd N.o:");
        scanf("%d",&c);
        int res;
        res=Subtract(y,c);
        printf("%d-%d=%d",y,c,res);
    }
    else if(x==3)
    {
        int y,c;
        printf("Multiplication\n");
        printf("Enter 1st N.o:");
        scanf("%d",&y);
        printf("Enter 2nd N.o:");
        scanf("%d",&c);
        int res;
        res=Multiplication(y,c);
        printf("%d*%d=%d",y,c,res);
    }
    else if(x==4)
    {
        int y,c;
        printf("Division\n");
        printf("Enter 1st N.o:");
        scanf("%d",&y);
        printf("Enter 2nd N.o:");
        scanf("%d",&c);
        float res;
        res=Divide(y,c);
        printf("%d/%d=%f",y,c,res);
    }
    else if (x>4)
    {
        printf("You Entered an Invalid Choice");
    }
}
int Add(int a,int b)
{
    int sum;
    sum=a+b;
    return sum;
}
int Subtract(int a,int b)
{
    int subtract;
    subtract=a-b;
    return subtract;
}
int Multiplication(int a,int b)
{
    int multiply;
    multiply=a*b;
    return multiply;
}
int Divide(int a,int b)
{
    float Div;
    Div=a/ b;
    return Div;
    
}
