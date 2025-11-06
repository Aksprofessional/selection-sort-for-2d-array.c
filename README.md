# selection-sort-for-2d-array.c

// selection sort for 2d array.
#include <stdio.h> 

int main() {
    int i,j,t;
    int a[2][3]={6,8,2,9,4,25};
    
    for(i=0;i<6;i++)
     for(j=0;j<=6;j++)
      if(*(*a+i)>*(*a+j)){
          t=*(*a+i);
          *(*a+i)=*(*a+j);
          *(*a+j)=t;
      }
     for(i=0;i<2;i++){
      for(j=0;j<3;j++)
         printf("%d  ",a[i][j]);
      printf("\n");
     }
    return 0;
}
