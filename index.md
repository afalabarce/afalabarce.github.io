#  afalabarce

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

## Mis desarrollos

Durante todos mis años desarrollando aplicaciones, he publicado varios de ellos, opensource la mayoría... entre ellos... destacan los siguientes (tanto opensource, como cerrados):

* *Java beans*, eran unos java beans que desarrollé hace ya casi 15 años, que permitían, utilizando NetBeans, el desarrollo de interfaces de Usuario en Java de una forma muy sencilla, extendiendo los Beans proporcionados por Swing, dotándolos de nuevas funcionalidades. El más destacado por su complejidad y funcionalidad, era un Grid (heredaba de JTable) que permitía de una forma visual (y sin escribir una sola línea de código) la configuración de dicho componente, dotándolo de funcionalidades directas como ordenación, formateo de tipos de celdas, celdas de agrupación, celdas de tipos primitivos y complejos, pintado condicional de celdas, etc.

* *MsSql2PgSql*, era un pequeño programa en Java, que permitía exportar una base de datos Sql Server (tablas y vistas) a PostgreSql, su funcionamiento era extremadamente sencillo. Una pequeña captura de pantalla puede hacer una idea de lo que permitía hacer...
<img width="646" alt="image" src="https://user-images.githubusercontent.com/103461358/194409037-e1e32d4e-2467-493c-a522-b38c97574eb5.png">

* *Aplicaciones Android*, he realizado a lo largo de los años (desde 2012) de forma personal 14 apps android, la mayoría por desgracia, ya no están disponibles, si bien cada una de ellas ocupa un lugar especial, por uno u otro motivo:
    *  *Parchis*, esta fue la primera, era un sencillo juego de parchís que realicé en un par de semanas.
    *  *El Juego de la Oca*, después del parchís lo natural era hacer la Oca, en este caso, ya que pude aprovechar la mayor parte del parchís, fue un visto y no visto.
    *  *My Checkout*, esta fue un auténtico reto, ya que... mediante Scrap accedía a la página de Checkout de Google (antigua pasarela de pagos de google para desarrolladores) a fin de proporcionar estadísticas y resultados de ventas de apps. Estuvo muy chula, la verdad...
    *  *Fm Radio Recorder*, esta app fue algo curioso, que surgió como una apuesta... tenía en su momento un Samsung galaxy S, el cual, permitía escuchar la radio pero no grabarla... entonces surgió la apuesta de que no se podía realizar la grabación de las emisoras... pero investigando un poco por Xda Developers, me encontré un artículo que explicaba con todo lujo de detalles la api de Samsung para la radio FM... el resultado... una app que era capaz de sintonizar una emisora, y grabarla, como en los viejos tiempos se grababan a casette las canciones de las emisoras favoritas... La app grababa en wav, y la última versión a ogg.
    *  *En 2013 se produjo un punto de inflexión*, y es que, me hice cliente del operador móvil Simyo, el cual en ese momento no disponía de app móvil (pocas operadoras tenían su propia app), entonces... les pedí permiso para realizar una app no oficial, permiso que me dieron (siempre eternamente agradecido a la compañía, y son totalmente recomendables). El resultado... *Mi Simyo*, una app que era capaz de conectar (imero por scrap a su web, y posteriormente mediante su API oficial), extraer y presentar de forma ordenada (incluidos diversos gráficos) los da.tos de facturación del cliente, permitiendo incluso la descarga de las facturas. Esta app es con diferencia a la que tengo más cariño de todas las que he podido desarrollar. Su evolución a lo largo de los años puede verse en la siguiente imagen:
	![image](https://user-images.githubusercontent.com/103461358/194412306-f91fd4d9-dda4-4db4-a8d4-6ade53cc064e.png)
    *  *My Jobs for Infojobs*, esta app nace de la participación en un concurso promovido por la plataforma de empleo de Infojobs, en ella se pedía realizar una app con algunas funcionalidades que permitiesen a un candidato gestionar tanto su curriculum como sus ofertas de empleo. La última versión de la app, era capaz, a partir de los datos de Infojobs, generar un curriculum en PDF que podía ser compartido con los contactos del usuario.
    *  *Mi Pomodoro*, esta es una de las últimas apps que he desarrollado, está desarrollada con las tecnologías de JetPack Compose, siendo la primera app que hago con esta tecnología de manera personal (que no profesional, ya que profesionalmente, ya había desarrollado 3 apps utilizando dicha tecnología). Es una app de tipo pomodoro, para gestionar los tiempos de trabajo empleados en tareas, así como los tiempos de descanso necesarios.
    *  *Palabras en cadena*, esta es la app más reciente que he desarrollado, es una app tipo Wordle, con la salvedad de que cada día disponemos de una partida completa con más de 9000 palabras españolas en las que cada palabra se relaciona con la anterior a partir de una de las letras. Ha sido muy satisfactorio realizarla, ya que además de JetPackCompose, he utilizado otras tecnologías tan interesantes como Inyección de dependencias con Hilt, Flows, etc. Ha sido muy divertido desarrollarla 😇

