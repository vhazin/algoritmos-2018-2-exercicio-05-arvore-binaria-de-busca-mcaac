#include <stdio.h>
#include <stdlib.h>

typedef struct No{
    int info;
    struct No *esq;
    struct No *dir;
}TNo;

typedef struct Arvore{
    TNo *raiz;
}TArvore;

void criar(TArvore *arvore){
TNo *novo;
novo = malloc(sizeof(TNo));
novo->info=aux;
novo->esq =NULL;
novo->dir=NULL;
  
}
int inserir_elemento(TArvore *arvore){

scanf("%d",aux);

    if(arvore->raiz == NULL){
      criar(TArvore *arvore)
        
    }
    else{
        if((novo->info)<(t->info)){
          inserir_elemento(&Ar)
            
        }
        else{
          inserir_elemento(&Ar)
          
        }

    }
}
int pre_ordem(TArvore *arvore){
    TNo *aux;
    aux = arvore->raiz;

    if(arvore!=NULL){
            printf("%d",aux->info);
            pre_ordem(aux->esq);
            pre_ordem(aux->dir);
        }
}

int in_ordem(TArvore *arvore){
    TNo *aux;
    aux = arvore->raiz;
    
        if(arvore!=NULL){
            pre_ordem(aux->esq);
            printf("%d",aux->info);
            pre_ordem(aux->dir);
        }
    
}

int pos_ordem(TArvore *arvore){
    TNo *aux;
    aux = arvore->raiz;
    
    if(arvore!=NULL){
            pre_ordem(aux->esq);
            pre_ordem(aux->dir);
            printf(" %d",aux->info);
        }

}



int x=0, z=0, j, i;
int main(){
    TArvore Ar;

    scanf("%d",&j);
    
    while(z<j){
        scanf("%d",&i);
        while(x<i){
            inserir_elemento(&Ar);
            x++;
        }
        printf("Case %d:",(z+1));
        printf("\nPre.:");
        pre_ordem(&Ar);
        printf("\nIn.:");
        in_ordem(&Ar);
        printf("\nPost.:");
        pos_ordem(&Ar);

    z++;
    }
    
printf("\n");
}
