#include<stdio.h>
 int n,s[10000]={0},ct=0;
 int bfs(int i)
 {
     int k,j=0,l,max=0;
     if(i>=n-1) return 0;    //找到便退出
     k=s[i];ct++;
     if(i+k>=n-1) return 0; //找到便退出

     for(l=i+1;l<=i+k;l++)   //for()找到下次能跳到最远的距离
     {
         
          if(max<=l+s[l])     //更新数据
         {
             j=l;max=l+s[l];      
         }
     }
     
     bfs(j);          //跳到最远的数组里
     
 }
 int main()
 {
     int i;
     scanf("%d",&n);
     for(i=0;i<n;i++)
     {
         scanf("%d",&s[i]); 
     }
     bfs(0);
     printf("%d",ct);    //打印步数
     return 0;
 }
