# menu_drivenCS
not complete
/******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <stdio.h>
void matrix_read();
void matrix_sum();
void matrix_product();
void matrix_transpose();
void display_matrix();
void main()
{
int choice,a[100][100],i,r;
printf("1.To read a matrix\n2.To add to matirx\n3.To multiply two matrix\n4.To find transpose\n5.To display a matrix\n");
scanf("%d",&choice);
if(choice==1){
    a=matrix_read();
    for(i=0;i<r;i++){
        for (j=0;j<c;j++){
        printf("%d\t",a[i][j]);
        
            
        }
        printf("\n");
    }
    
}
else if(choice==2){
    matrix_sum();
}
else if(choice==3){
    matrix_product();
    
}
else if(choice==4){
    matrix_transpose();
}
else if(choice==5){
    display_matrix();
}
else{
    printf(" Wrong command ");
}
}
int matrix_read(){
    int i,j,r,c,a[100][100];
    printf("Enter the no. of rows: ");
    scanf("%d",&r);
    printf("Ënter the no. of columns: ");
    scanf("%d",&c);
    printf("Enter the values: ");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            scanf("%d",&a[i][j]);
        }
    }
    return a;
    
    
    
}



void matrix_sum(){

    int i,j,r,c,a[100][100,b[100][100],sum[100][100];
    printf("Enter the no. of rows of matrix: ");
    scanf("%d",&r);
    printf("Ënter the no. of columns of matrix: ");
    scanf("%d",&c);
    printf("Enter the values of first matrix: ");
        for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            scanf("%d",&)a[i][j]);
        }
    }
            
    printf("Enter the values of second matrix: ");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            scanf("%d",&b[i][j]);
        }
    }
    
    for(i=0;i<r;i++){
        for (j=0;j<c;j++){
        sum[i][j]=a[i][j]+b[i][j];
            
        }
    }
    for(i=0;i<r;i++){
        for (j=0;j<c;j++){
        printf("%d\t",sum[i][j]);
        
            
        }
        printf("\n");
    }
    
    
    
    
}

void matrix_product(){
    int i,j,r,c2,c,a[100][100,b[100][100],sum[100][100],count;
    printf("Enter the no. of rows of matrix: ");
    scanf("%d",&r);
    printf("Ënter the no. of columns of matrix: ");
    scanf("%d",&c);
    printf("Enter the values of first matrix: ");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            scanf("%d",&a[i][j]);
        }
    }
    
    printf("for multiplication row should be same as that of previous column \n");
    
    printf("Enter the columns of second matrix: ");
    scanf("%d",&c2);
    printf("Enter the values of second matrix: ");
    for(i=0;i<r;i++){
        for(j=0;j<c2;j++){
            scanf("%d",&a[i][j]);
        }
    }
    
    for(i=0;i<r;i++){
        countrow=0;
        countcol=0;
        for(j=0;j<c;j++){
          p[countrow][countcol]+=a[i][j] * b[j][i];
          countcol += 1;
          
        }
        countrow += 1;
    }
    
    for(i=0;i<r;i++){
        for(j=0;j<c2;j++){
            printf("%d\t",p[i][j]);
        }
        printf("\n");
    }
    
    
    
}

void matrix_transpose(){
    int i,j,r,c,a[100][100],t[100][100];
    printf("Enter the no. of rows: ");
    scanf("%d",&r);
    printf("Ënter the no. of columns: ");
    scanf("%d",&c);
    printf("Enter the values: ");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            scanf("%d",&a[i][j]);
        }
    }
    
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            t[i][j] = a[j][i];
        }
    }
    
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            printf("%d\t",t[i][j]);
        }
        printf("\n");
    }
}

int display_matrix(a[100][100]){
    int i,r;
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            printf("%d\t",a[i][j]);
        }
        printf("\n");
    }
}
    
    
