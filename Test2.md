```c
#include <iostream>

int a[100000];
int b[100000];
int main() {
  int dis, money, n, temp;

  scanf("%d" ,&n);

  for(int i = 0; i < n-1; i++)
    scanf("%d", &a[i]);
  for(int i = 0; i < n; i++)
    {
      scanf("%d", &b[i]);
      dis += b[i];
    }  

  money = a[0] * dis;
  for(int i = 0; i < n-1; i++)
    {
     temp += a[i] * b[i];
    }
  temp += a[n];
  if(temp < money)
    money = temp;
    

  
}
```
