```c
#include <iostream>

int main() {
  int a,b;
  long long v;
  scanf("%d %d %lld", &a,&b,&v);

  int temp = 0;
  int res = 1;
  while(1)
    {
      temp += a;
      if(temp < v)
      {
        temp -= b;
        res++; 
      }
      else if(temp >= v)
        break;
    }
  printf("%d", res);
}
```
