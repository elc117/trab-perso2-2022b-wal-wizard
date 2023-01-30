![pattern](https://user-images.githubusercontent.com/82295321/215579427-5ff2bb04-bfdc-488d-8539-40f4e5978841.png)

## Definição - o que significa Pattern Matching  ?

A correspondência de padrões na ciência da computação é a verificação e localização de sequências específicas de dados de algum padrão entre dados brutos ou uma sequência de tokens. Ao contrário do reconhecimento de padrões, a correspondência deve ser exata no caso de correspondência de padrões. A correspondência de padrões é um dos paradigmas mais fundamentais e importantes em várias linguagens de programação. Muitos aplicativos usam a correspondência de padrões como uma parte importante de suas tarefas.

## Examplo: 

```
object Demo {
   def main(args: Array[String]) {
      val alice = new Person("Alice", 25)
      val bob = new Person("Bob", 32)
      val charlie = new Person("Charlie", 32)
   
      for (person <- List(alice, bob, charlie)) {
         person match {
            case Person("Alice", 25) => println("Hi Alice!")
            case Person("Bob", 32) => println("Hi Bob!")
            case Person(name, age) => println(
               "Age: " + age + " year, name: " + name + "?")
         }
      }
   }
   case class Person(name: String, age: Int)
}
```

## Comando para executar o código

```
\>scalac Demo.scala
\>scala Demo
```
## Saida
```
Hi Alice!
Hi Bob!
Age: 32 year, name: Charlie?
```


## Dentre as inúmeras utilidades do Pattern Matching, as que mais se destacam são:
  - Procura em uma coleção de documentos de texto (Aqui basicamente poderemos fazer uma varredura em um arquivo e retornando apenas o que queremos)
  - Procua em um documento XML 

