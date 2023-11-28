#include<stdio.h>
int solve(long long int n){
     int sum=0;
     while (n != 0){
          int p = n%10;
          if(p==4 || p == 7)sum++;
          n/=10;
     }

      if (sum == 4 || sum == 7)return 1;
      return 0;
}
 int main (){
     long long int n;
     scanf("%lld",&n);
     if (solve(n) == 1)printf("YES\n");
     else printf("NO\n");
     }
