#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>
int main()
{
    int a, b;
    printf("输入成绩");
    scanf("%d %d", &a, &b);
    int sum = a + b, tag;
    if (a < 0 || a > 100 || b < 0 || b > 100)
    {
        printf("错误\n");
    }
    else
    {
        sum = a + b;
        if (sum >= 180)
            tag = 0;
        else if (sum >= 160)
            tag = 1;
        else if (sum >= 140)
            tag = 2;
        else if (sum >= 120)
            tag = 3;
        else
            tag = 4;
        switch (tag)
        {
        case 0:
            printf("%d----> A\n", sum);
            break;
        case 1:
            printf("%d----> B\n", sum);
            break;
        case 2:
            printf("%d----> C\n", sum);
            break;
        case 3:
            printf("%d----> D\n", sum);
            break;
        case 4:
            printf("%d----> E\n", sum);
            break;
        }
    }
    return 0;
}
