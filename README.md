#include <stdio.h>

int main(){ 
    int n,i,j;
    printf("\n Enter the size of 1st array ");
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++){
        printf("\n Enter the %d element of the array",i+1);
        scanf("%d",&a[i]);
    }
    int m;
    printf("\n Enter the size of 2nd array");
    scanf("%d",&m);
    int b[m];
    for(i=0;i<m;i++){
        printf("\n Enter the %d element of the array",i+1);
        scanf("%d",&b[i]);
    }
    int c[20],k=0;
    for(i=0;i<n;i++){
    for(j=0;j<m;j++){
        if(a[i]==b[j]){
            break;
        }
    }
        if(j==m){
            c[k]=a[i];
            k++;
        }
        
    }
    for(i=0;i<n-2;i++){
        printf("%d",c[i]);
    }
        
        
    
    return 0;
}
