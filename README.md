Ngoài cách lấy <img src="https://render.githubusercontent.com/render/math?math=\sqrt n"> các bạn có thể sử dụng 1 đặc điểm của số chính phương để giải : số chính phương khi chia 8 luôn dư 0 hoặc 1 hoặc 4.
<details>
  <summary>AC code</summary>
  
  ```c
#include <stdio.h>

typedef  long long int64;
typedef char bool;
bool true = 1;
bool false = 0;

bool isSquare(int64 n)	{
    if (n < 0)
        return false;
    else if (n%8 == 0 || n%8 == 1 || n%8 == 4)
        return true;
    return false;
}

int main()	{
    
    int64 n;
    scanf("%lld", &n);

    if (isSquare(n))
        printf("YES");
    else
        printf("NO");

    return 0;
}
  ```
</details>
