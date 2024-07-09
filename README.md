#include <stdio.h>

int main() {
    int x, y, z;
    int *px, *py, *pz, *tmp;

    printf("x");
    scanf("%d", &x);
    printf("y");
    scanf("%d", &y);
    printf("z");
    scanf("%d", &z);

    px = &x;
    py = &y;
    pz = &z;

    tmp = px;
    px = py;
    py = pz;
    pz = tmp;


    printf("%d, %d, %d\n", *px, *py, *pz);

    return 0;
}
