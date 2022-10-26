#  afalabarce

## Sobre mi

¡Hola! me llamo Antonio Fernández, procedo de un pequeño pueblo de la costa granadina llamado [Ítrabo](https://es.wikipedia.org/wiki/%C3%8Dtrabo) (sí, es un nombre un poco "raro" :D) aunque por cosas de la vida, resido en Almería (España), y soy desarrollador en múltiples plataformas y lenguajes, entre las que me apasionan (y se llevan el tiempo que puedo dedicar):
* .Net Framework y .Net Framework Core (con C# como lenguaje)
* Desarrollo nativo con Android (utilizando Kotlin principalmente, aunque he vivido la época Java, de la que guardo gratos recuerdos)
* SQL, sobre todo, utilizando bases de datos Sql Server, PostgreSql (QUE ME ENCANTA ❤️) Y MySql (y sus clones)
* Estoy empezando también a hacer mis pinitos con Flutter, aunque Dart (me reservo mi opinión )... 
* Otros lenguajes, con los que he jugado, Python, Swift, Javascript (aunque como curiosidad y con intención didáctica)

Mi Historia con el desarrollo de aplicaciones comienza a la edad de 11 años, con un ordenador [Amstrad PC 1512DD (IBM Compatible)](https://es.wikipedia.org/wiki/Amstrad_PC1512), el lenguaje Basic (Locomotive Basic2), y una curiosidad que me hizo aprender a desarrollar mi primer juego (un Ahorcado) como un pequeño pique sano con un familiar. 
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

Este hobby infantil se convirtió en mi gran pasión y mi profesión, previo paso por la [Universidad de Granada](https://www.ugr.es). 

De la [Escuela Técnica Superior de Ingeniería Informática](https://etsiit.ugr.es/) guardo unos recuerdos increibles, de toda la gente que conocí, tanto compañeros de estudios como profesores, que de un modo u otro, marcaron mi forma de ser e incentivaron esa curiosidad que ya tenía aquel chaval de 11 años, que utilizaba su primer ordenador con la ilusión de ver que aquello que escribía en un idioma "extraño" provocaba que el aparato hiciese lo escrito (más o menos 🙃)


Como no todo en la vida es desarrollar software, tengo otras aficiones (evidentemente) :
- La lectura (tengo entre manos la trilogía de Marte, entre otros), de la cual me apasiona el género de Ciencia Ficción principalmente.
- El buen cine, el cine clásico me encanta, Erol Flinn, Burt Lancaster, Chaplin (especialmente me encanta el Gran Dictador), además de comedias y de acción, claro está.
- Dar laaaaargos paseos con mi Perrita, que es incansable, lo que la convierte en la compañera ideal para esas caminatas 😅

![image](https://user-images.githubusercontent.com/103461358/194420396-6f3ed5e4-d353-4de2-954c-a3ebecfb3f5b.png)



## Mis desarrollos

Durante todos mis años desarrollando aplicaciones, he publicado varios de ellos, opensource la mayoría... entre ellos... destacan los siguientes (tanto opensource, como cerrados):

* *Java beans*, eran unos java beans que desarrollé hace ya casi 15 años, que permitían, utilizando NetBeans, el desarrollo de interfaces de Usuario en Java de una forma muy sencilla, extendiendo los Beans proporcionados por Swing, dotándolos de nuevas funcionalidades. El más destacado por su complejidad y funcionalidad, era un Grid (heredaba de JTable) que permitía de una forma visual (y sin escribir una sola línea de código) la configuración de dicho componente, dotándolo de funcionalidades directas como ordenación, formateo de tipos de celdas, celdas de agrupación, celdas de tipos primitivos y complejos, pintado condicional de celdas, etc.

![image](https://user-images.githubusercontent.com/103461358/194666078-98554e61-d99b-433b-b833-5433a2897046.png)
![image](https://user-images.githubusercontent.com/103461358/194666191-0ea30301-542c-4600-96bd-f34a8554b934.png)
![image](https://user-images.githubusercontent.com/103461358/194666249-c229f20d-a6cb-48b1-a1cd-6157e56226aa.png)

* *MsSql2PgSql*, era un pequeño programa en Java, que permitía exportar una base de datos Sql Server (tablas y vistas) a PostgreSql, su funcionamiento era extremadamente sencillo. Una pequeña captura de pantalla puede hacer una idea de lo que permitía hacer...
* 
<img width="646" alt="image" src="https://user-images.githubusercontent.com/103461358/194409037-e1e32d4e-2467-493c-a522-b38c97574eb5.png">

* *Aplicaciones Android*, he realizado a lo largo de los años (desde 2012) de forma personal 14 apps android, la mayoría por desgracia, ya no están disponibles, si bien cada una de ellas ocupa un lugar especial, por uno u otro motivo:
    *  *Parchis*, esta fue la primera, era un sencillo juego de parchís que realicé en un par de semanas.
    
![image](https://user-images.githubusercontent.com/103461358/194415683-9dd44dcd-11d6-454d-bfa4-f45336035be2.png)
   
   *  *El Juego de la Oca*, después del parchís lo natural era hacer la Oca, en este caso, ya que pude aprovechar la mayor parte del parchís, fue un visto y no visto.
    
![image](https://user-images.githubusercontent.com/103461358/194416292-a3f7fa09-4a18-4077-bc17-0eaf4f9511d1.png)
   
   * *El Juego de la Escalera*, este fue otro jueguecillo de desarrollo rápido, que aprovechaba prácticamente el 90% de la lógica de la Oca... :D

![image](https://user-images.githubusercontent.com/103461358/194429052-a85c1af3-4bfd-4fa4-af52-4b5fe1ece276.png)


   *  *My Checkout*, esta fue un auténtico reto, ya que... mediante Scrap accedía a la página de Checkout de Google (antigua pasarela de pagos de google para desarrolladores) a fin de proporcionar estadísticas y resultados de ventas de apps. Estuvo muy chula, la verdad...
    
![image](https://user-images.githubusercontent.com/103461358/194416420-3ec4048c-f746-4458-90b4-6132ffacc76a.png)
   
   *  *Fm Radio Recorder*, esta app fue algo curioso, que surgió como una apuesta... tenía en su momento un Samsung galaxy S, el cual, permitía escuchar la radio pero no grabarla... entonces surgió la apuesta de que no se podía realizar la grabación de las emisoras... pero investigando un poco por Xda Developers, me encontré un artículo que explicaba con todo lujo de detalles la api de Samsung para la radio FM... el resultado... una app que era capaz de sintonizar una emisora, y grabarla, como en los viejos tiempos se grababan a casette las canciones de las emisoras favoritas... La app grababa en wav, y la última versión a ogg.
    
![image](https://user-images.githubusercontent.com/103461358/194415960-dc810cea-7b4b-405d-8cec-c89f05337f7f.png)
    
   *  *En 2013 se produjo un punto de inflexión*, y es que, me hice cliente del operador móvil Simyo, el cual en ese momento no disponía de app móvil (pocas operadoras tenían su propia app), entonces... les pedí permiso para realizar una app no oficial, permiso que me dieron (siempre eternamente agradecido a la compañía, y son totalmente recomendables). El resultado... *[Mi Simyo](https://play.google.com/store/apps/details?id=com.tarsys.miSimyo)*, una app que era capaz de conectar (primero por scrap a su web, y posteriormente mediante su API oficial), extraer y presentar de forma ordenada (incluidos diversos gráficos) los da.tos de facturación del cliente, permitiendo incluso la descarga de las facturas. Esta app es con diferencia a la que tengo más cariño de todas las que he podido desarrollar. Su evolución a lo largo de los años puede verse en la siguiente imagen:
    
![image](https://user-images.githubusercontent.com/103461358/194412306-f91fd4d9-dda4-4db4-a8d4-6ade53cc064e.png)
   
   *  *My Jobs for Infojobs*, esta app nace de la participación en un concurso promovido por la plataforma de empleo de Infojobs, en ella se pedía realizar una app con algunas funcionalidades que permitiesen a un candidato gestionar tanto su curriculum como sus ofertas de empleo. La última versión de la app, era capaz, a partir de los datos de Infojobs, generar un curriculum en PDF que podía ser compartido con los contactos del usuario.
    
![image](https://user-images.githubusercontent.com/103461358/194416604-ef2ae5aa-b6ab-481b-9ece-255062fdb3f6.png)
   
   *  *[Mi Pomodoro](https://play.google.com/store/apps/details?id=io.github.afalabarce.mypomodoro)*, esta es una de las últimas apps que he desarrollado, está desarrollada con las tecnologías de JetPack Compose, siendo la primera app que hago con esta tecnología de manera personal (que no profesional, ya que profesionalmente, ya había desarrollado 3 apps utilizando dicha tecnología). Es una app de tipo pomodoro, para gestionar los tiempos de trabajo empleados en tareas, así como los tiempos de descanso necesarios.
    
![image](https://user-images.githubusercontent.com/103461358/194416716-e4703223-798e-45fb-b12b-4ab0485a96c8.png)
   
   *  *[Palabras en cadena](https://play.google.com/store/apps/details?id=io.github.afalabarce.wordlepuzzle)*, esta es la app más reciente que he desarrollado, es una app tipo Wordle, con la salvedad de que cada día disponemos de una partida completa con más de 9000 palabras españolas en las que cada palabra se relaciona con la anterior a partir de una de las letras. Ha sido muy satisfactorio realizarla, ya que además de JetPackCompose, he utilizado otras tecnologías tan interesantes como Inyección de dependencias con Hilt, Flows, etc. Ha sido muy divertido desarrollarla 😇
    
![image](https://user-images.githubusercontent.com/103461358/194416797-3f57076d-f5ac-48bf-b5a4-60be98b1dad9.png)


## Desarrollos OpenSource

Además de las apps desarrolladas, tengo varios repositorios en Github en los que bajo licencia Open Source, pongo a disposición de la comunidad algunos desarrollos que creo pueden ser útiles (a mi me resultan útiles, por lo que seguro que al menos a otro desarrollador podrán servirle):

- *[Tutorial de despliegue en Maven Central](https://github.com/afalabarce/DeployToMavenCentralTutorial)*, este repo no lleva nada de código, sólo es un tutorial paso a paso en el que se describe el método para desplegar nuestros desarrollos de librerías en MavenCentral, a fin de poder ponerlos a disposición de la comunidad, por ejemplo en Android Studio.
- *[ORM Propio escrito en Java](https://github.com/afalabarce/TaRSySAndroidORM)*, este repo contiene un ORM que desarrollé en Java, cuando no teníamos Room, que permitía de una forma relativamente sencilla la utilización y explotación de datos sin utilizar ni una sola sentencia SQL (incluso las migraciones las ejecutaba solo).
- *[ORM Propio escrito en Kotlin](https://github.com/afalabarce/TaRSySAndroidORMKotlin)*, el mismo ORM que el anterior, pero adaptado a Kotlin, con algunas funcionalidades extra, que pude implementar gracias a las particularidades de Kotlin, a día de hoy no tiene sentido su uso, aunque como material didáctico puede resultar muy muy útil.
- *[NetCoreWebApi](https://github.com/afalabarce/NetCoreWebApi)*, este repo contiene un servicio web básico Rest realizado con .Net Core, que despliega lo mínimo necesario para permitir un desarrollo, esto es implementa como mínimo la autenticación mediante tokens JWT. El servicio soporta como motores de bases de datos a Sql Server, PostgreSql y MySql (y derivados).
- *[Cajón Desastre](https://github.com/afalabarce/mess_drawer)*, este repositorio lo he pensado como un cajón desastre, en el que agregaré pequeños desarrollos que, por un motivo u otro, no he agregado a otros repositorios, actualmente tiene una implementación de un Dialog para navegación por sistemas de archivos mediante *JetPack Compose para escritorio* (sin utilizar ninguna integración Swing).
- *[Componentes JetPack Compose](https://github.com/afalabarce/jetpackcompose)*, este repositorio es al que más tiempo dedico y el que más funcionalidades dispone, todas pensadas para el sistema de UI JetPackCompose:
	- *CalendarComposable*, implementa un componente CalendarPicker, así como un CalendarDropDown, de muy fácil configuración y despliegue.
	- *CircularProgressIndicator*, implementa un ProgressIndicator circular, que permite agregar composables en el interior del toroide, al que además agrega un fondo de color en la zona no completada.
 	- *DrawCanvas*, implementa un canvas de dibujo, al que además he agregado la posibilidad de agregar una marca de agua, al estilo de un sello, pudiendo estar delante o detrás del trazo realizado.
	- *LabelledSwitch*, es un switch para compose, que permite asignar tanto un label como un leadingIcon al switch (compose sólo nos da el propio switch, sin label.
	- *ModifierExtensions*, son unas extensiones al modifier de compose, que nos permite modificar los bordes de un composable, dandole un formato de punteado de líneas.
	- *NoPaddingAlertDialog*, este composable nos permite utilizar un AlertDialog SIN paddings (en compose los AlertDialog tienen un padding (que no se puede quitar) de 16.dp. De este modo, podemos personalizar enormemente su apariencia.
	- *SpinnerSelector*, otro composable que compose no proporciona, en este caso, el "clásico desplegable".
	- *SwipeableCard*, este composable nos permite, mediante desplazamientos horizontales, agregar diversas acciones a un card, de este modo es muy sencillo, e intuitivo el acceso a múltiples opciones.
	- *ViewModelService*, este desarrollo es un Service que implementa el acceso a ViewModel, por lo que podemos crear servicios que van a poder comportarse de forma reactiva.
	
	Para utilizar estos composables, es taaaaan sencillo como en el build.gradle de tu app poner lo siguiente	
	
	```groovy
	// dependiendo de cuando lo leas, esta versión habrá subido, ya que tendrá nuevos composables...
	implementation "io.github.afalabarce:jetpackcompose:1.3.2" 
	```


## Conclusión


Si has llegado hasta aquí, mil gracias por aguantar las parrafadas anteriores, en caso de que quieras contactar conmigo, puedes hacerlo por ejemplo, a través de [Mi perfil en LinkedIn](https://www.linkedin.com/in/antonio-f-83415069/)

Un saludo!!!
