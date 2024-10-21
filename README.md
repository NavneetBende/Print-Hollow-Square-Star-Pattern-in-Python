PRINTING PATTERN:
****

*    *

*    *

****

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take number of rows/columns as input from the user (length of side of square) and store it in any variable (‘l’ in this case).
Run  a loop ‘l’ number of times to iterate through all the rows. From i=0 to i<l. The loop should be structured as for( i=0; i<l ; i++).
Run a nested loop inside the main loop for printing stars . From j=0 to j<l. The loop should be structured as for( j=0 ; j<l : j++).
Inside the above loop print stars only if  i=0 or i=l-1 or j=0 or j=l-1 in all other cases print a blank space.
Move to the next line by printing a new line. printf(“\n”).
Code in C:
#include<stdio.h>
int main()
{
int i,j,l;    //declaring integers i,j for loops and l for the number of rows
printf(" Enter the number of rows\n");   //Asking user for input
scanf("%d",&l);   //taking input for number of rows and saving in variable l
for(i=0;i<l;i++) //Outer loop for number of rows
   {
      for(j=0;j<l;j++) //Inner loop for printing stars in each column of a row
         {
            if(i==0 || i==l-1 || j==0 || j==l-1) // condition for printing stars
               {
                  printf("*");   // printing stars
               }
            else                 // else condition to print spaces 
               {
                  printf(" ");   //printing spaces
               }
         }
      printf("\n");       //Printing a new line after a row has been printed
   }
}
TAKING INPUT:
DISPLAYING OUTPUT:
