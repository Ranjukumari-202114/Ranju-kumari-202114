# Ranju-kumari-202114




/*Write a  program to search an element in 2-D array using linear search method*/

#include<stdio.h>
int main()
{
   int n, m,search=0 ,i,j;
   printf("Enter the number of row in an array\n");
   scanf("%d", &m);
    printf("Enter the number of coloum in an array\n");
   scanf("%d", &n);
   int arr[m][n];
   printf("enter the element one by one\n");
   for(i=0; i<m; i++)
    { 
       for(j=0; j<n; j++)
         {
              printf("Enter the element of row %d column %d\n",i+1,j+1);
              scanf("%d", &arr[i][j]); 
         }
    }
   printf("Enter the element you want to find\n");
   int element;
   scanf("%d", &element);
   for(i=0; i<m; i++)
   { 
       for(j=0; j<n; j++)
         {
             if(arr[i][j]==element)
             {
              search=1;
              printf(" element found at row %d column %d\n",i+1,j+1);
                break; 
              }
              
          }
  
   }
   if(search==0)
   printf(" element not found in the array");
   return 0;
}
