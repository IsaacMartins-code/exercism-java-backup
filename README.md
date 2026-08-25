
# Exercism - Exercícios de código

![Java](https://img.shields.io/badge/Java-f08c00?style=flat&logo=openjdk&logoColor=white)
![C](https://img.shields.io/badge/-C_lang-00599C?style=flat&logo=c&logoColor=white)

Exercícios de código da plataforma [Exercism](https://exercism.org/profiles/IsaacMartins-code) realizados sem auxílio de IA, a fim de exercitar constantemente minha lógica de programação e minha capacidade de solução de problemas. Neste readme destaco os principais desafios que realizei na plataforma.

## 1. Diamond kata💎 - [ver o código](https://github.com/splinterdev/exercism-backup/blob/main/solutions/java/diamond/1/src/main/java/DiamondPrinter.java)
![Java](https://img.shields.io/badge/Java-f08c00?style=flat&logo=openjdk&logoColor=white)

Dada uma letra, é imprimido um losango começando com 'A', com a letra fornecida no ponto mais largo.
<br>
<br>
Este desafio me permitiu compreender como unicode de letras do alfabeto latino funcionam e como utilizar de algumas operações básicas e estruturas de repetição para construir o diamante.

### Exemplo

#### chamada do método na main e println com forEach:

```java
     public class Program {
       public static void main(String[] args) {
          DiamondPrinter printer = new DiamondPrinter();
          List<String> list = printer.printToList('F');

          list.forEach(System.out::Println);
       }
     }
```

#### Saída:

```
     A     
    B B    
   C   C   
  D     D  
 E       E 
F         F
 E       E 
  D     D  
   C   C   
    B B    
     A                           
```

## 2. Say📨 - [ver o código](https://github.com/splinterdev/exercism-backup/tree/main/solutions/java/say)
![Java](https://img.shields.io/badge/Java-f08c00?style=flat&logo=openjdk&logoColor=white)

> [!NOTE]
> Pasta do desafio contém várias subpastas com diferentes submissões de melhorias realizadas e a mais recente é a de número maior. Código deste desafio em específico ainda está sendo melhorado😅.

Dado um número, é retornado a sua expressão por extenso na lingua inglesa.
<br>
<br>
Este desafio me permitiu ver na prática passagem e manipulação de objetos em métodos por referência, além da reutilização de código.

### Exemplo

#### chamada do método na main e println:

```java
     public class Program {
       public static void main(String[] args) {
          Say say = new Say();
          String phrase = say.say(987_654_321_123L);

          System.out.println(phrase);
       }
     }
```

#### Saída:

```
nine hundred eighty-seven billion six hundred fifty-four million three hundred twenty-one thousand one hundred twenty-three
```

## 3. Grains🌽 - [ver código](https://github.com/splinterdev/exercism-backup/blob/main/solutions/java/grains/1/src/main/java/Grains.java)
![Java](https://img.shields.io/badge/Java-f08c00?style=flat&logo=openjdk&logoColor=white)

Desafio relacionado a lenda sobre o pedido de recompensa realizada por um servo a um rei, que consistia em um grão de trigo para a primeira casa do tabuleiro de xadrez e o dobro para cada próxima casa. No desafio, dado um número de uma casa do tabuleiro, é retornado a quantidade de grãos dessa casa. Também há um método que calcula a quantidade de grãos totais em um tabuleiro.

### Exemplo

#### chamada do método na main e println:

```java
     public class Program {
       public static void main(String[] args) {
          Grains grains = new Grains();

          System.out.println(grains.grainsOnSquare(16));
          System.out.println(grains.grainsOnBoard());
       }
     }
```

#### Saída de grãos em uma casa:

```
32768
```

#### Saída de grãos totais em um tabuleiro:

```
18446744073709551615
```
