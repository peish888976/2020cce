# 2020cce

找零錢，輸入n元，問會找多少50元,5元,1元
#include <stdio.h>
int main()
{
  int n;
  scanf("%d",&n);
  printf("%d=50*%d+5*%d+1*%d\n",n,n/50,n%50/5,n%50%5);
}

找倍數
#include <stdio.h>
int main()
{
  int n,k=0;
  for(int i=1,i<=10,i++)
  {
   scanf("%d",&n);
   if(n%3==0)
   {
     k++;
   }
  } 
  printf("%d\n",k);
}  

因數個數
#include <stdio.h>
int main()
{
  int n;
  scanf("%d",&n);
  int k=0;
  for(int i=1;i<=n;i++){
  if(n%i==0) k++}
  printf("%d\n",k);
