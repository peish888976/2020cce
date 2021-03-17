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

#include <stdio.h>
int a[5]={0,10,20,30,40};
int main()
{
   int *p=&a[2];
   *p=222;
   p=p+2;
   *p=666;
}

#include <stdio.h>
int a[5]={0,10,20,30,40};
void printfAll()
{
   for(int i=0;i<5;i++){
      printf("%d",a[i]);
   }
   printf("\n");
}
int main()
{
  int *p=&a[2];
  *p=222;
     printAll();
  *p=666;
     printAll()
  p--;
  *p=555;
  printAll();
  
}

#include <stdio.h>
int a[10]={0,10,20,30,40,50,60,70,80,90};
void printfAll()
{
   for(int i=0;i<10;i++){
      printf("%d",a[i]);
   }
   printf("\n");
}
int main()
{
  int *p=&a[2];
  *p=200;
     printAll();
     int *p2=p+4;
  *p2=666;
     printAll()
  p2--;
  *p2=555;
  printAll();
  return 0;
}
