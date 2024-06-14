#include <stdio.h>
void printUnion(int arr1[], int arr2[], int m, int n)
{
  int i = 0, j = 0;
  while (i < m && j < n) {
    if (arr1[i] < arr2[j])
     printf("%d ",arr1[i++]);

    else if (arr2[j] < arr1[i])
     printf("%d ",arr2[j++]);

    else {
     printf("%d ",arr2[j++]);
     i++;
    }
  }

  /* Print remaining elements of the larger array */
  while (i < m)
   printf("%d ",arr1[i++]);

  while (j < n)
   printf("%d ",arr2[j++]);
}

void printIntersection(int arr1[], int arr2[], int m, int n)
{
  int i = 0, j = 0;
  while (i < m && j < n) {
     if (arr1[i] < arr2[j])
      i++;
     else if (arr2[j] < arr1[i])
      j++;
     else /* if arr1[i] == arr2[j] */
     {
       printf("%d ",arr2[j]);
       i++;
       j++;
     }
    }
}

/* Driver program to test above function */
int main()
{ 
   int m, n;

   scanf("%d", &m);

   int arr1[m];

   for(int i=0; i<m; i++) scanf("%d", &arr1[i]);

   scanf("%d", &n);

   int arr2[n];

   for(int i=0; i<n; i++) scanf("%d", &arr2[i]);

   // Function calling
  printf("Union : ");
  printUnion(arr1, arr2, m, n);


  printf("\nIntersection ");
  printIntersection(arr1, arr2, m, n);

  return 0;
}
