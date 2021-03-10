# 2020cce
#include <stdio.h>
int main()
{
   int 1=10,n2=20,n3=30;
   printf(""n1:%d n2:%d n3:%d\n );
   int *p=&n1;             p1裡面放的是n1住址 &1
   *p=200;
   printf("n1:%d n2:%d n3:%d\n); 
    int *p2=&n3;
   *p2=300;                p2裡面放的是n3的位址 &n3
   printf("n1:%d n2:%d n3:%d\n); 
   p2=p;
   *p2=400;
   printf("n1:%d n2:%d n3:%d\n); 
   return 0;
}
