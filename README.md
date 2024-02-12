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
</br>

<!--comment diamond-->
_d_ __i__~~a~~`mond`

```c
#include<stdio.h>
int main()
{
    while(1)
    {
        int num,space,row,col;
        printf("Enter the number : ");
        scanf("%d",&num);

        for(row=1; row<num; row++)
        {
            for(space=1; space<=num-row; space++)
            {
                printf(" ");
            }

            for(col=1; col<=row; col++)
            {
                printf("%d",col);
            }

            for(col=1; col<row; col++)
            {
                printf("%d",col);
            }
            printf("\n");
        }

        for(row=num; row>=1; row--)
        {
            for(space=1; space<=num-row; space++)
            {
                printf(" ");
            }
            for(col=1; col<=row; col++)
            {
                printf("%d",col);
            }
            for(col=1; col<row; col++)
            {
                printf("%d",col);
            }
            printf("\n");
        }
    }
}
```

<image src="./images/diamond.png" width="500" title="diamond" />

continue ..