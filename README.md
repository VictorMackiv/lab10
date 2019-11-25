# lab10
#include<iostream>
#include<cstdlib>
#include<Windows.h>
using namespace std;
 
int main() {
    SetConsoleCP(1251);
    SetConsoleOutputCP(1251);
    float x,A,B,sum=0,S;
    while(1){
    printf("Continue? (1 - yes/ 0 - no) = ");
    fflush(stdout);
    scanf("%f",&x);
    if(x==1){
        printf("\nValue A = ");
        fflush(stdout);
        scanf("%f",&A);
        printf("Value B = ");
        fflush(stdout);
        scanf("%f",&B);
        if(A==B){
            for(S=A;S<=B;S=S+0.1){
                sum=S+sum;
                printf("Value = %1.1f\n",S);
                printf("%f\n",sum);
                if(S>=0&&(S - int(S)) == 0){
                    int i,res=1;
                    for(i=1;i<=S;i++){
                        res*=i;
                    }
                    printf("факториал = %d",res);
 
                    }}
                }
 
 
        if(A<B){
                for(S=A;S<=B;S=S+0.1){
                sum=S+sum;
                printf("Value = %1.1f\n",S);
                printf("Sum = %1.3f\n",sum);
                if(S>=0&&(S - int(S)) == 0){
                    int i,res=1;
                    for(i=1;i<=S;i++){
                    res*=i;
                        }
                    printf("факториал = %d\n",res);
 
                }}}
 
        if(A>B){
                    for(S=B;S<=A+0.1;S=S+0.1){
                    sum=S+sum;
                    printf("Value = %1.1f\n",S);
                    printf("Sum = %1.3f\n",sum);
                    if(S>=0&&(S - int(S)) == 0){
 
                                int i,res=1;
                                for(i=1;i<=S;i++){
                                    res*=i;
                                }
                                printf("факториал = %d",res);
 
                                }}
    }}
    else if(x==0){
        break;
    }else{
        continue;
    }
    }
    return 0;
}
