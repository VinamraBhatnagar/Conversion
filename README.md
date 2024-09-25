#include<stdio.h>
int main(){
    int rem;
    int n;
    int i=0;
    int a[15];
    int selection;
    printf("1.Decimal to binary\n");
    printf("2.Decimal to octal\n");
    printf("3.Decimal to Hexadecimal\n");
    printf("enter your selection:");
    scanf("%d",&selection);
    if(selection==1){
        printf("enter the value:");
    scanf("%d",&n);
    while (n)
    {
        rem=n%2;
        n=n/2;
        a[i]=rem;
        i++;
    }
    for(int j=i-1;j>=0;j--){
         printf("%d",a[j]);
    }
    }
    else if(selection==2){
        printf("enter the value:");
    scanf("%d",&n);
    while (n)
    {
        rem=n%8;
        n=n/8;
        a[i]=rem;
        i++;
    }
    for(int j=i-1;j>=0;j--){
         printf("%d",a[j]);
     }
    }
    else if(selection==3){
        printf("enter the value:");
    scanf("%d",&n);
    while (n)
    {
        rem=n%16;
        n=n/16;
        a[i]=rem;
        i++;
    }
    for(int j=i-1;j>=0;j--){
         printf("%d",a[j]);
    }
    }
    else{
        printf("invalid input");
    }
     return 0;
 }
