

is bad!!!!



#define _CRT_SECURE_NO_WARNINGS
#include <stdlib.h>
#include <stdio.h>
#define row 4
#define colume 4

int main()
{
    int y, x, a, b, c, d, r, s, sum1 = 0, sum2 = 0;
    int mtrx[row][colume] = { {1,5,6,4}, {11,9,1,8}, {6,4,11,12}, {13,7,7,10} };
    int mtrx1[row][colume] = { {1,5,6,4}, {11,9,1,8}, {6,4,11,12}, {13,7,7,10} };

    for (x = 0; x < colume; x++)
    {
        for (y = 0; y < row; y++)
        {
            for (a = 0; a < colume; a++)
            {
                for (b = 0; b < row; b++)
                {

                    sum1 = mtrx[x][y] + mtrx1[a][b];
                    printf("sum1 -> %d \n", sum1);

                    for (x = 0; x < colume; x++)
                    {
                        for (y = 0; y < row; y++)
                        {
                            for (a = 0; a < colume; a++)
                            {
                                for (b = 0; b < row; b++)
                                {
                                    sum2 = mtrx[x][y] + mtrx1[a][b];
                                    printf("sum2 -> %d \n", sum2);

                                    if (sum1 = sum2)
                                    {
                                        printf("%d and %d..\n", sum1, sum2);
                                    }
                                }
                            }
                        }
                    }
                }
            }
        }
    }
}
