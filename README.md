### Caso Base

- O caso base é a condição que interrompe a recursão para ser executada infinitamente.

- Quando ```n == 1``` ou ```n == 0``` a função não precisa mais se chamar novamente, pois já sabemos que o fatorial de 1
  e de 0 é 1.

- Por conta disto simplemente retornamos 1 e encerramos a recursão.

### Passo Recursivo

- No passo recursivo, a função chama a si mesma para resolver um problema menor.

- A ideia é:

```text
fatorial(n) = n * fatorial(n - 1)
```

- Esse processo continua reduzindo o problema ate chegar no caso base, onde a recurção para.

### Rastreio das Chamadas

| Etapa | Chamada                       | Retorno |
|:------|:------------------------------|:--------|
| 1     | fatorial(4) → 4 × fatorial(3) | ?       |
| 2     | fatorial(3) → 3 × fatorial(2) | ?       |
| 3     | fatorial(2) → 2 × fatorial(1) | ?       |
| 4     | fatorial(1) → 1               | 1       |
| 5     | 2 × 1                         | 2       |
| 6     | 3 × 2                         | 6       |
| 7     | 4 × 6                         | 24      |

- Resultado final: ```4! = 24```
