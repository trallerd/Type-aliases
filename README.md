# Type-aliases
### Entendendo e aplicando *[Type Aliases](https://kotlinlang.org/docs/reference/type-aliases.html)* em Kotlin.
![](https://www.sngular.com/wp-content/uploads/2019/11/Kotlin-Blog.png)
Type Aliases, se trata de uma forma de abreviar e/ou renomear o codigo, para obter um código mais limpo e legível!

> When type definitions distract from what your code means because they’re not readable, expressive or just too long, Kotlin has just the right feature for you: typealias! Typealias allows you to provide alternate names for class or functions types without introducing a new type.(
[Florina Muntenescu](https://medium.com/androiddevelopers/alter-type-with-typealias-4c03302fbe43))

Para facilitar a escrita do seu codigo, você pode ultilizar type aliases em:

- Encurtar longos tipos :

`typealias MapString = Map<String, String>`

- Nos tipos de função||parametros||retornos:

*ultilizando o exmplo acima*

`fun printMap(map: MapString){
  for((key, value) in map){
        println(value)
    }
}`

- Novos nomes para inner e nested classes:

`typealias BarBeer = Bar.beer
class Bar {
    private val name: String = "TheBar"
    inner class beer {
    }
}`


> Lembrando também que ao utilizar typealias nenhum tipo novo é criado. Em tempo de compilação o alias é substituído pelo seu tipo final. Assim, não há nenhum peso adicional no bytecode com o uso deles.([Diego Malone](https://medium.com/concretebr/type-alias-e-inline-class-em-kotlin-b7c6b276851d))



### About me
[![Github Badge](https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/fagnerpsantos)](https://github.com/Trallerd)
[![Twitter Badge](https://img.shields.io/badge/-Twitter-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/trallerd)](https://twitter.com/trallerd)
[![Youtube Badge](https://img.shields.io/badge/-YouTube-ff0000?style=flat-square&labelColor=ff0000&logo=youtube&logoColor=white&link=https://www.youtube.com/channel/UCHmlPQF6AVr3y7fj7TE-7Hw)](https://www.youtube.com/channel/UCHmlPQF6AVr3y7fj7TE-7Hw)
