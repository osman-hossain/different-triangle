<!--comment-->
Different way to print triangle or pyramid

```c
#include<stdio.h>
int main()
{
    int num,row,col,space;
    printf("Enter the number : ");
    scanf("%d",&num);

    for(row=1; row<=num; row++)
    {
        for(space=1; space<=num-row; space++)
        {
            printf(" ");
        }

        for(col=1; col<row; col++)
        {
            printf("%d",col);
        }

        for(col=row; col>=1; col--)
        {
            printf("%d",col);
        }
        printf("\n");
    }
return 0;
}

```

![pic](./images/pic.png)