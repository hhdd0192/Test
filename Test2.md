```c
#include <iostream>

int a[100000];
int money[100000];
int main() {
  int n, total, temp;

  scanf("%d" ,&n);

  for(int i = 1; i < n; i++)
    scanf("%d", &a[i]);
  for(int i = 0; i < n; i++)
      scanf("%d", &money[i]);

  temp = money[0];
  total = temp + a[1];

  for(int i = 1; i < n; i++)
    {
      if(temp < money[i])
        total += temp + money[i-1];
      else
      {
        temp = money[i];
        total += temp + money[i+1];
      }
    }
  printf("%d", total);
    

  
}
```
