# 05-02

c언어로 만든 주사위 프로그램

```c
#include <stdio.h>
#include <stdlib.h>
#include <conio.h>
#include <time.h>

int main() {
    int dice;

    srand(time(NULL));

    while (1) {
        printf("아무키나 눌러 주사위 굴리기\n\n");
        _getch();

        dice = rand() % 6 + 1;

        if (dice == 1) {
            printf("■■■■■■■■■\n■              ■\n■              ■\n■              ■\n■      ■      ■\n■              ■\n■              ■\n■              ■\n■■■■■■■■■\n\n주사위 값은 1!\n\n");
        }

        else if (dice == 2) {
            printf("■■■■■■■■■\n■              ■\n■   ■         ■\n■              ■\n■              ■\n■              ■\n■         ■   ■\n■              ■\n■■■■■■■■■\n\n주사위 값은 2!\n\n");
        }

        else if (dice == 3) {
            printf("■■■■■■■■■\n■              ■\n■   ■         ■\n■              ■\n■      ■      ■\n■              ■\n■         ■   ■\n■              ■\n■■■■■■■■■\n\n주사위 값은 3!\n\n");
        }

        else if (dice == 4) {
            printf("■■■■■■■■■\n■              ■\n■   ■    ■   ■\n■              ■\n■              ■\n■              ■\n■   ■    ■   ■\n■              ■\n■■■■■■■■■\n\n주사위 값은 4!\n\n");
        }

        else if (dice == 5) {
            printf("■■■■■■■■■\n■              ■\n■   ■    ■   ■\n■              ■\n■      ■      ■\n■              ■\n■   ■    ■   ■\n■              ■\n■■■■■■■■■\n\n주사위 값은 5!\n\n");
        }

        else if (dice == 6) {
            printf("■■■■■■■■■\n■              ■\n■   ■    ■   ■\n■              ■\n■   ■    ■   ■\n■              ■\n■   ■    ■   ■\n■              ■\n■■■■■■■■■\n\n주사위 값은 6!\n\n");
        }

    }

    return 0;
}

```
