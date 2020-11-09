#include <stdio.h>
#define MAX 5
int q[MAX];
int p[MAX];
int rear1=-1;
int front1=-1;
int rear2=-1;
int front2=-1;
int i;
void enque1(int ele)
{
    
      rear1=(rear1+1)%MAX;
      q[rear1]=ele;
      printf("%d enqueued in q\n",ele);
      if(front1 ==-1)
          front1=0;
      
}
void enque2(int ele)
{
    
      rear2=(rear2+1)%MAX;
      p[rear2]=ele;
      printf("%d enqueued in p\n",ele);
      if(front2 ==-1)
          front2=0;
      
}
void display()
{
    printf("the elements divisible by all numbers from 1 to 10 are ");
    for(i=front2;i<=rear2;i++)
    {
       printf("%d\t", p[i]);
    }
}
int main()
{
    int item;
    
    printf("enter the queue elements\t");
    for(i=0;i<MAX;i++)
    {
        scanf("%d",&item);
        enque1(item);
    }
    for(i=front1;i<=rear1;i++)
    {
        if((q[i]%2==0)&&(q[i]%3==0)&&(q[i]%4==0)&&(q[i]%5==0)&&(q[i]%6==0)&&(q[i]%7==0)&&(q[i]%8==0)&&(q[i]%9==0)&&(q[i]%10==0))
        {
          enque2(q[i]);  
        }
    }
    display();
    return 0;
}
