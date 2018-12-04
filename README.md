# Structure_Array
Contains the record of Students and Prints in tabular form:


#include <stdio.h>
#include <stdlib.h>
#include <string.h>

void main()
{
    int n,i;

  struct student
  {
      int roll;
      char name[50];
      int fees;
  }s1[n];

  printf("Enter the number of students: \n");
  scanf("%d",&n);

 

  for(i=1;i<=n;i++)
  {
      printf("Enter the Roll- \n");
      scanf("%d",&s1[i].roll);

       printf("Enter the Name- \n");
      scanf("%s",s1[i].name);

       printf("Enter the Fee Amount- \n");
      scanf("%d",&s1[i].fees);

  }

   printf("NAME \t ROLL \t FEE \n");

  for(i=1;i<=n;i++)
  {
      printf("%s \t %d \t %d \n",s1[i].name, s1[i].roll, s1[i].fees);
  }
}

