# 第一天課程

## C語言開發
nano 文字編輯器
```
nano <檔案>
```
ctrl+X 後選擇 Y 按 enter 保存後退出

編譯
```
gcc <C程式碼檔案> -o <輸出名稱>
```
執行
```
./<執行檔>
```

### 範例一：Hello World
```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

### 範例二：if 判斷式
```c
#include <stdio.h>

int main() {
    int height;
    printf("Please enter your height:");
    scanf("%d", &height);

    if(height >= 190){
        printf("Too high\n");
    }
    else if (height == 180){
        printf("Perfect!\n");
    }
    else{
        printf("Too Short\n");
    }
    return 0;
}
```

### 範例三：for 迴圈
```c
#include <stdio.h>

int main() {
    for(int i=0;i<10;i++){
        printf("%d\n", i);
    }
    return 0;
}
```

### 範例四：遞增運算子
```c
#include <stdio.h>

int main() {
    int a = 12;
    a++;
    printf("%d\n", a);
    ++a;
    printf("%d\n", a);
    return 0;
}
```

### 範例五：遞迴函式
```c
#include <stdio.h>

int function(int x){
    if(x == 0)
        return 0;
    else if(x == 1)
        return 1;
    else
        return function(x-1)+function(x-2);
}

int main() {
    int num;
    scanf("%d", &num);
    printf("%d", function(num));
    return 0;
}
```

### 課間練習：Bit 操作
a = 12, b = 9
請撰寫一個程式找出以下四值
a AND b
a OR b
a XOR b
NOT a

提示：
```c
#include <stdio.h>

int main() {
    int a = 12;
    int b = 9;
    printf("%d\n", a & b);
    printf("%d\n", ?????);
    printf("%d\n", ?????);
    printf("%d\n", ?????);
    return 0;
}
```

### 範例六：指標
```c
#include <stdio.h>

int main() {
    int a=2;
    int *ptr;
    ptr = &a;
    printf("a: %d \n", a);
    printf("ptr: %p \n", ptr);
    printf("*ptr: %d \n", *ptr);
    return 0;
}
```
### 範例七：傳遞參數給 main
```c
#include <stdio.h>

int main(int argc, char *argv[]) {
    printf("Number of arguments: %d\n", argc); 

    for (int i = 1; i < argc; i++) {
        printf("Argument %d: %s\n", i, argv[i]);
    }

    return 0;
}
```
