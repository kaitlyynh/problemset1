# problemset1



#include <cs50.h>
#include <stdio.h>

int main(void)
{
    //get integer from person  domain:[1,8]
    int n;
    do
    {
      n = get_int("Height? ");  
    }
    while (n < 1 || n > 8);
    // the main for loop represents ROWS. i=0 is row 1, i=1 is row 2, etc., increasing by increments of 1
    for (int  i = 0; i < n; i++)
    {
        // the inner for lloops (the J integer) is COLUMNS. j=0 is column 1. 
        for (int j=0; j < n; j++)
        {
            if ((i + j) < n - 1)
            printf("");
            else
            printf("#");
            
        }
        printf("\n");
    }
    
}
