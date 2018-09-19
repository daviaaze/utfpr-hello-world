# Este é um título
## Este é um subtitulo

+ Este é um item de uma lista
+ Este é outro item de uma lista

```c
  \#include <stdio.h>
  \#include <stdlib.h>

  struct pesquisa {
    int idade;
    char sexo;
    float renda;
    int filhos;
  };

  int main(int argc, char const *argv[]) {
    int i = 0;
    float media = 0;
    int contag = 0;
    struct pesquisa p[20];
     for (i = 0; i < 20; i++) {
      printf("Idade: ");
      scanf("%i", &p[i].idade);
      printf("Sexo: ");
      scanf(" %c", &p[i].sexo);
      printf("Renda: ");
      scanf("%f", &p[i].renda);
      printf("Filhos: ");
      scanf("%i", &p[i].filhos);
     }
     for (i = 0; i < 20; i++) {
     media = media + p[i].renda;
     if (p[i].sexo == 'f' && p[i].filhos > 2 && p[i].renda < 600.00) {
       contag++;
     }
     }
     media = media / 20.0;
     printf("A media da renda e de R$%.00f\n e as mulheres com mais de dois filhos e renda a baixo de R$600.00 e %i", media, contag);
      return 0;
  }
```
