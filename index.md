#
## Sobre mi

¡Hola! me llamo Antonio Fernández, y soy desarrollador en múltiples plataformas y lenguajes, entre las que me apasionan (y se llevan el tiempo que puedo dedicar):
* .Net Framework y .Net Framework Core (con C# como lenguaje)
* Desarrollo nativo con Android (utilizando Kotlin principalmente, aunque he vivido la época Java, de la que guardo gratos recuerdos)
* SQL, sobre todo, utilizando bases de datos Sql Server, PostgreSql (QUE ME ENCANTA ❤️) Y MySql (y sus clones)
* Estoy empezando también a hacer mis pinitos con Flutter, aunque Dart (me reservo mi opinión )... 
* Otros lenguajes, con los que he jugado, Python, Swift, Javascript (aunque como curiosidad y con intención didáctica)

Mi Historia con el desarrollo de aplicaciones comienza a la edad de 11 años, con un ordenador Amstrad PC 1512DD (IBM Compatible), el lenguaje Basic (Locomotive Basic2), y una curiosidad que me hizo aprender a desarrollar mi primer juego (un Ahorcado) como un pequeño pique sano con un familiar. 
La siguiente aplicación que desarrollé fue una calculadora, que como toda calculadora empezó con las operaciones básicas, hasta que con 14 años, gracias a un reto de mi profesor de Matemáticas... diseñé y programé un triángulo de Tartaglia (pongo el código en Kotlin a continuación, bastante más breve que con basic 😇):

```kotlin
import java.util.*
import java.text.*

// Referencia: https://www.estadisticaparatodos.es/taller/triangulo/triangulo.html
// 
fun Int.factorial(): Int =  if (this > 1) this * (this - 1).factorial() else 1
fun combPascal(n: Int, m: Int): Int = m.factorial() / (n.factorial() * (m - n).factorial())


fun main() {
	val valorM = 4
    val siPotenciado = false
    
    for(m in 0..valorM){
        for (n in 0..m){
            if (siPotenciado)
            	print("($n,$m) ")
            else
            	print("${combPascal(n,m)} ")
        }
        println("")
    }
}
```

Este hobby infantil se convirtió en mi gran pasión y mi profesión, previo paso por la Universidad de Granada. 

De la Escuela Técnica Superior de Ingeniería Informática guardo unos recuerdos increibles, de toda la gente que conocí, tanto compañeros de estudios como profesores, que de un modo u otro, marcaron mi forma de ser e incentivaron esa curiosidad que ya tenía aquel chaval de 11 años, que utilizaba su primer ordenador con la ilusión de ver que aquello que escribía en un idioma "extraño" provocaba que el aparato hiciese lo escrito (más o menos 🙃)
