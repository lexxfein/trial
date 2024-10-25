#include <stdio.h>
int po(int n,int p);

int main(){

    int n,p;
    printf("enter n,p: ");
    scanf("%d%d",&n,&p);
    printf("%d",po(n,p));

    return 0;
}

int po(int n,int p){
    if(p==0){
        return 1;
    }
    if(p==1){
        return n;
    }
    int o;
    o=po(n,p-1)*n;
    return o;
}
