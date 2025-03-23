# Curso de Vue.js: Introducción y Fundamentos

## Índice
* [Clase 01 - ¿Qué es Vue.js?](#id1)
* [Clase 02 - Fundamentos de Componentes](#id2)
* [Clase 03 - Configuración del entorno](#id3)
* [Clase 04 - Primer Contacto](#id4)
* [Clase 05 - Interpolación de datos](#id5)
* [Clase 06 - Interpolación de datos Parte 2](#id6) 
* [Clase 07 - Atributos reactivos](#id7)
* [Clase 08 - Eventos de usuario](#id8)

---

## ¿Qué es Vue.js? [1/22]<a name="id1"></a>
Vue.js es uno de los frameworks de desarrollo frontend más relevantes en la actualidad. Creado por **Evan Yu**, quien tiene experiencia en gigantes del desarrollo como Google, Vue.js combina lo mejor de mundos como Angular y ReactJS. Su enfoque se centra en ofrecer una herramienta profesional, de fácil acceso al ser 100% open source, lo que significa que está completamente a disposición de la comunidad de desarrolladores. Este modelo comunitario no solo fomenta la innovación, sino que también enriquece el ecosistema de herramientas, utilidades y librerías que complementan a Vue.js.

### ¿Por qué elegir Vue.js?
* **Open Source**: Al no estar vinculado a ninguna empresa, es una plataforma completamente abierta, lo que garantiza flexibilidad y libertad de uso.
* **Comunidad Activa**: La comunidad alrededor contribuye continuamente al crecimiento y mejora del framework.
* **Popularidad en GitHub**: Su repositorio en GitHub es uno de los más populares, reflejándose en el alto número de estrellas que posee.

### Comenzando con Vue.js: Primeros pasos y sintaxis básica
El primer paso es comprender su sintaxis básica y la creación de componentes reutilizables. La estructura modular de Vue.js lo hace accesible para proyectos nuevos y ya existentes. Los desarrolladores pueden implementar componentes de código reutilizable para mejorar la eficiencia y consistencia en sus aplicaciones.

### ¿Cómo utilizar Vue.js en proyectos existentes?
1. Integración básica: permite una fácil integración en sistemas existentes gracias a su diseño modular.
2. Desarrollo de componentes: La creación de componentes es sencilla, lo que facilita su reutilización en distintos puntos de una aplicación, promoviendo prácticas de desarrollo eficiente.
3. Ecosistema robusto: Las herramientas y librerías disponibles complementan su uso, ampliando las posibilidades de aplicación en proyectos complejos.

### Explorando la sintaxis de Vue.js
Destaca por su sintaxis intuitiva que simplifica el desarrollo frontend.
+ **Componentes**: La creación y manejo de componentes es central en este framework.
+ **Directivas**: Estas son esenciales para manipular el DOM de manera eficiente.
+ **Reactividad**: Ofrece un sistema reactivo que sincroniza automáticamente los cambios en los datos con la interfaz de usuario.

--- 

## Fundamentos de componentes [2/22]<a name="id2"></a>

### ¿Qué es el desarrollo basado en componentes?
Es un enfoque moderno en la creación de software que prioriza la creación de componentes independientes que interactúan entre sí. Esta metodología no se limita exclusivamente al desarrollo web, sino que también se aplica a otras áreas de desarrollo de software.
+ **Abstracción de componentes**: Se busca encapsular partes de un software, como una pasarela de pagos o un carrito de compra, en componentes aislados que se comunican a través de una interfaces.
+ **Interoperabilidad**: La interfaz actúa como un contrato estandarizado que permite la comunicación entre componentes, facilitando el desarrollo independiente y la evolución del sistema.
+ **Reutilizabilidad**: Los componentes pueden ser sustituidos o mejorados sin afectar al sistema global, optimizando el mantenimiento y evolución del software.

### ¿Qué son los componentes de UI?
Los componentes de interfaz de usuario (User Interface) son elementos visuales con los que los usuarios interactúan en una aplicación o página web. Estos pueden ser nativos en HTML o creados mediante frameworks como Vue.js, React.js, o Angular.
* Tipos comunes de componentes: Incluyen botones, formularios, calendarios y más. Algunos componentes, como los calendarios, evolucionaron para permitir funcionalidades más avanzadas, como el manejo de rangos de fechas, vital para aplicaciones de reserva de vuelos o alojamiento.
* Implementación de componentes: Utilizar frameworks permite crear componentes personalizados repetibles, encapsulando la lógica necesaria para que sean fácilmente reutilizables en diferentes partes de una aplicación.

### Ejemplo de un componente en HTML

````html
<input type="date" value="2023-03-15">
````

Este es un ejemplo básico de un campo de entrada de fecha en HTML que se ve visualmente diferente dependiendo del navegador o del dispositivo móvil.

### ¿Cuáles son las principales partes de un componente de UI?
La estructura y funcionamiento de un componente UI dentro de un framework son:
+ **Vista**: Es la parte visible e interactiva con la que los usuarios interactúan; incluye botones y otros elementos visuales.
+ **Estado**: Los componentes pueden cambiar entre diferentes estados según las interacciones del usuario o la configuración de la aplicación. Un botón, por ejemplo, puede estar activado o desactivado, cambiando visualmente de color o quedando desactivado.
+ **Interfaz**: Los componentes se comunican con el resto del sistema mediante eventos y atributos, como 'onClick', para ejecutar funciones específicas en respuesta a interacciones del usuario.

### ¿Cómo funciona el patrón MVVM?
El patrón Model-View-ViewModel (MVVM) se utiliza en frameworks de desarrollo para separar la lógica de negocio de la interfaz de usuario.
+ **Modelo (Model)**: Contiene la lógica de negocios y los datos de la aplicación.
+ **Vista (View)**: La interfaz de usuario visible.
+ **VistaModelo (ViewModel)**: Actúa como intermediario, sincronizando la vista con el modelo y permitiendo que las actualizaciones en uno se reflejen automáticamente en el otro.

### Sincronización de datos con Vue.js
El proceso de mantener sincronizados el modelo y la vista a través de **Two-Way Data Binding**. Esto permite que cualquier cambio en el modelo se refleje inmediatamente en la vista y viceversa.

* Ventajas: Evita la necesidad de manipular directamente el DOM con JavaScript, simplificando el proceso de desarrollo y mejorando la eficiencia.
* Un ejemplo seria: Cambios en un objeto de datos (como un JSON) se reflejan en los componentes UI vinculados, y las interacciones del usuario actualizan automáticamente el modelo sin intervención manual.

Este enfoque moderno simplifica el desarrollo y mantenimiento, permitiendo crear aplicaciones robustas y flexibles con menos esfuerzo.

---

## Fundamentos de componentes [3/22]<a name="id3"></a>

### ¿Cómo preparar el entorno de desarrollo para trabajar con Vue.js?
Iniciar un proyecto en Vue.js requiere que tengamos algunas herramientas bien configuradas en nuestro entorno de desarrollo. Es esencial tener conocimientos básicos de JavaScript, HTML y desarrollo web. Además, se debe tener instalado Node.js y un editor de código, de preferencia Visual Studio Code.

### ¿Qué instalar?
* Instalar la version mas estable de Node.js

> [!NOTE]
> El profesor estará usando la version 16.13

* Instalar las devtools de Vue desde la tienda de chrome, para ello ir a la [pagina oficial](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd?hl=ES). Este plugin nos permitirá realizar la inspección de elementos de sitios desarrollados con Vue JS.
* Abrir visual studio code, abrir una terminal de comandos y ejecutar el siguiente comando:
`npm install -g @vue/cli`

### ¿Cómo añadir Vue.js a través de un CDN?
Un CDN (Content Delivery Network) te permite incluir Vue.js rápidamente, ideal para proyectos simples.
Agregar el CDN como aparece en la [documentación oficial](https://vuejs.org/guide/quick-start#using-vue-from-cdn) dentro de una etiqueta **script** en el html.
La estructura de un proyecto Vue debería quedar de la siguiente manera:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>

    <div id="app"></div>

    <script>
        // Aquí ira el código de VueJS
    </script>
</body>
</html>
```

---

## Primer Contacto [4/22]<a name="id4"></a>

### ¿Cómo crear un componente Vue.js?
Para empezar a utilizar Vue.js en una aplicación web, se deben seguir estos pasos:
1. Agregar el script que hará el llamado al CDN de Vue para comenzar a utilizarlo (este debe ser declarado dentro del *body* del documento index):
````html
<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
````
2. Crear una estructura HTML: Se define un elemento *div* con un id único. Para este ejemplo sera:
````html
<div id="app"></div>
````
3. Desarrollar un componente: se declara nuevamente una etiqueta *script* y dentro se comenzara a agregar la lógica utilizando Vue y JavaScript.

Aquí es donde se comienza a desarrollar un proyecto

````html
<div id="app"></div>
<script>
    const app = Vue.createApp({ 
	/* Aquí definiremos opciones más adelante */ 
	});
    app.mount('#app');
</script>
````

### ¿Qué es la options API y cómo utilizarla?
Vue.js se destaca por su facilidad de uso, en parte debido a la options API. Esta es una forma estructurada de definir componentes que utiliza objetos JSON para describir la funcionalidad del componente.

### Uso de la opción data
La opción **data()** suele ser la puerta de entrada para gestionar el estado en un componente se usa de la siguiente forma:

````javascript
const app = Vue.createApp({
    data() {
        return {
            text: 'Hola, Vue'
        }
    }
});
````

Con la option API, se pueden definir variables que serán reactivas. En este ejemplo, text es la variable que puede ser usada dentro del HTML mediante doble llaves {{ text }}.

### Montaje y automatización de la vista
Una vez que definas las variables dentro de **data()**, Vue.js automáticamente sincroniza los cambios. Esto significa que si el estado cambia, la vista se actualizará sin necesidad de manipular el DOM de manera tradicional.

### ¿Cómo funciona la reactividad en Vue.js?
La magia de Vue.js radica en su habilidad de actualizar la vista automáticamente cuando cambian los datos. El metodo **createApp()** no solo inicializa una aplicación, sino que devuelve un objeto conocido como **view model** que mantiene sincronizada la vista y el modelo.

### Ventajas de Vue.js para proyectos web
1. Reactividad: Cambios de datos que automáticamente actualizan el DOM.
2. Progresivo: Comienza con funcionalidades básicas que pueden expandirse según sea necesario.
3. Opciones robustas de configuración: La options API permite una descripción clara y estructurada del comportamiento deseado.
4. Convenciones comunitarias: Se recomiendan sugerencias por la comunidad en el uso de variables como *vm* para el ViewModel, lo cual ayudara en la lectura y entendimiento del código por parte de otros desarrolladores.

---

## Interpolación de datos [5/22]<a name="id5"></a>
Uno de los aspectos más poderosos de Vue.js es la interpolación de datos, que permite integrar dinámicamente variables de JavaScript dentro de nuestro HTML. Al entender y utilizar esta característica, se podra construir aplicaciones interactivas y reactivas, maximizando tanto funcionalidad como rendimiento.

### ¿Qué es la interpolación en Vue.js?
Es una técnica que permite insertar y visualizar datos de forma dinámica en el HTML. Utilizando llaves dobles **{{ }}**, y dentro se puede insertar cualquier expresión de JavaScript válida o datos que provengan del contexto de datos de Vue, como variables y propiedades del componente. Por ejemplo:

````html
<div>{{ text }}</div>
````

En este caso, la variable *text* se interpolará en el lugar de las llaves dobles, haciendo visible su contenido en la vista en el navegador.

### ¿Cómo manejar los componentes y aplicaciones en Vue.js?
Una aplicación se maneja a través de un objeto principal que puede contener múltiples componentes. Este objeto, a menudo nombrado **vm** (abreviatura de ViewModel), es la instancia de la aplicación Vue y contiene toda la lógica e interacciones.

Existen dos enfoques para manejar aplicaciones con múltiples componentes:
1. Crear instancias separadas: Utilizar **Vue.createApp()** para generar instancias independientes.
2. Componentes anidados: Este enfoque es más común, ya que permite contener subcomponentes dentro de un componente principal, compartiendo contexto, acceso a datos y lógicas comunes.

### ¿Qué considerar al insertar expresiones en HTML?
Al utilizar la interpolación, es importante mantener el código limpio y organizado. Aunque se puede insertar cualquier expresión JavaScript dentro de las llaves dobles {{ }}, se recomienda separar la lógica compleja para evitar enredar el código:
1. Evitar lógica compleja: Insertar solo expresiones simples.
2. Separar las preocupaciones: Mantener la lógica JavaScript fuera de las vistas.

---

## Interpolación de datos Parte 2 [6/22]<a name="id6"></a>
La forma más común de utilizar la interpolación de datos es mediante el uso de dobles llaves ({{ }}) dentro de las vistas. Sin embargo, existe una opción más poderosa y flexible: el uso de **Templates** en cada componente. 
Los templates permiten definir la estructura del HTML de un componente mientras integran directivas de Vue.js, extendiendo así las capacidades del HTML convencional.

### ¿Cómo funcionan las directivas de Vue.js?
Las directivas son una manera poderosa de agregar funcionalidad a los componentes de Vue.js. Se declaran directamente en el template, lo que permite modificar o extender el comportamiento de los elementos HTML de manera declarativa. Estas directivas, como v-text, v-once y v-html, comienzan con "**v-**" seguido de su nombre específico y pueden recibir argumentos.

### ¿Qué es la directiva v-text?
La directiva v-text se utiliza para insertar texto directamente en un elemento HTML evitando el uso de las llaves dobles. Esta directiva ofrece una forma más declarativa y evita errores de sintaxis al utilizar expresiones JavaScript cuando no son necesarias. Por ejemplo, en lugar de {{ text }}, se utiliza una variación como la siguiente:

````html
<div v-text="text"></div>
````

### Otros tipos de directivas
+ **v-once**: Esta directiva hace que una parte del template se renderice solo una vez. Cualquier cambio en los datos asociados no actualizará la vista, útil para elementos no reactivos.
+ **v-html**: Similar a v-text, pero con la capacidad de insertar HTML sin escapar las etiquetas. Por razones de seguridad, se debe tener cuidado al insertar contenido que podría provenir de usuarios, para evitar vulnerabilidades de seguridad como la inyección de scripts maliciosos (como XSS).

### ¿Cómo asegurar el uso de v-html?
Es fundamental manejar v-html con precaución, especialmente cuando el contenido potencialmente proviene de entradas de usuarios. Por ejemplo, en formularios donde los datos se almacenan en bases de datos y se redistribuyen a diferentes usuarios, no utilizar v-html es una buena práctica para evitar la ejecución de código malintencionado. En su lugar, se sugiere usar datos provenientes de fuentes seguras, como HTML generado por el servidor o configuraciones predefinidas no editables por los usuarios.

### Recomendaciones al usar Vue.js
* Evitar usar directivas con valores de usuarios: No utilizar directivas como v-html con contenido que provenga de usuarios no confiables.
* Documentarse en la fuente oficial: Explorar la documentación oficial de Vue.js donde se pueden encontrar listas detalladas de directivas y sus aplicaciones.
* Práctica segura: Siempre monitorizar cualquier código introducido en v-html y otras directivas similarmente flexibles que puedan representar un riesgo de inyección de código.

---

## Atributos reactivos [7/22]<a name="id7"></a>
Gestionar la renderización de datos en la vista de un componente es una tarea esencial en cualquier aplicación dinámica, y Vue.js ofrece herramientas poderosas para hacerlo.
Pero, ¿qué sucede cuando necesitamos más que solo mostrar datos, y queremos manipular atributos HTML de manera dinámica? Ahí es donde entra en juego la directiva **v-bind**, una herramienta que permite modificar los valores de los atributos de HTML de forma reactiva y eficiente.

### ¿Qué es y cómo se utiliza la directiva v-bind?
La directiva v-bind es una función esencial en Vue.js que facilita la modificación de los atributos HTML en componentes. Con v-bind, se puede hacer que los atributos de los elementos HTML sean dinámicos, enlazándolos a las propiedades de datos declaradas dentro de un componente.

### Ejemplo de utilización de v-bind
Se desea usar una imagen en HTML a la cual se le debe asignar dinámicamente tanto su url (source) como su texto alternativo (alt). Con v-bind se puede hacer de manera sencilla:

````html
<template>
  <img v-bind:src="img" v-bind:alt="imgAlt">
</template>

<script>
export default {
  data() {
    return {
      img: 'https://example.com/image.jpg',
      imgAlt: 'Descripción alternativa de la imagen'
    }
  }
}
</script>
````

En este ejemplo, en lugar de insertar la URL de forma estática, v-bind permite usar variables, haciendo el código más flexible y reactivo.

### ¿Cómo se pueden utilizar argumentos dinámicos?
Desde la versión 3 de Vue.js, v-bind permite utilizar argumentos dinámicos. Esto significa que se puede enlazar la directiva a una variable que determine qué atributo se va a modificar, lo que añade una capa extra de flexibilidad.
Si esto lo llevamos a un ejemplo en codigo: utilizando el mismo codigo del ejemplo anterior, ahora se desea que el atributo que se está modificando también sea dinámico:

````html
<template>
  <img v-bind:[dynamicAttr]="img">
</template>

<script>
export default {
  data() {
    return {
      img: 'https://example.com/image.jpg',
      dynamicAttr: 'src'
    }
  }
}
</script>
````

Esta sintaxis permite que el valor de *dynamicAttr* en data() determine qué atributo de la etiqueta *img* se está gestionando.

### Ventajas de usar Vue.js para manipular atributos HTML
Utilizar v-bind para manipular atributos HTML ofrece diversas ventajas como:
* Reactividad: Los cambios en los datos del componente se reflejan inmediatamente en la interfaz de usuario sin necesidad de actualizar manualmente.
* Optimización de Código: Reduce la necesidad de manejar el DOM directamente con JavaScript Vanilla, lo que simplifica el código y aumenta su mantenibilidad.
* Escalabilidad: Facilita la creación de componentes reutilizables y dinámicos, adaptables a diferentes contextos y necesidades funcionales.
* Facilidad de Aprendizaje: Vue.js tiene una curva de aprendizaje corta, lo cual permite a los desarrolladores empezar a ser productivos rápidamente.

---

## Eventos de usuario [8/22]<a name="id8"></a>
La programación reactiva transformó la forma en que construimos interfaces de usuario, y Vue.js es uno de los frameworks que ha aprovechado esta potencia para crear experiencias de usuario dinámicas e interactivas.

### ¿Cómo escuchar eventos de usuario con Vue.js?
Existen directivas potentes para gestionar eventos de usuario sin necesidad de manipular directamente el DOM como lo haríamos con JavaScript puro. Entre ellas, v-on es esencial. Para escuchar los eventos se deben seguir los siguientes pasos:

1. Definición de un componente: En Vue.js, los eventos de usuario se gestionan mayormente a través de directivas. Se inicia creando un botón que reaccionará a un evento click.
````html
<template>
  <button v-on:click="increment">counter</button>
</template>
````
2. Declaración de métodos: Vue.js utiliza un objeto **methods** en el que se definen las acciones que se quieren realizar cuando un evento suceda.
````javascript
methods: {
  increment: function() {
    console.log('click');
  }
}
````
3. Manipular el DOM sin JavaScript nativo: Vue.js facilita la escucha de eventos sin el uso de manipulación directa del DOM, integrando scripts automáticamente en la estructura del código.

### ¿Cómo lograr reactividad con eventos en Vue.js?
Comprender y manejar adecuadamente la reactividad es clave para aprovechar al máximo las capacidades de Vue.js. Aquí hay algunos pasos para reaccionar a eventos de manera reactiva.

1. Variables reactivas: Utilizar el objeto data() para definir variables reactivas.
````javascript
data() {
  return {
    counter: 0
  }
}
````
2. Uso de this: Al manejar eventos, se puede acceder a valores dentro del componente a través de this.
````javascript
methods: {
  increment: function() {
    this.counter++;
  }
}
````

Cada vez que el botón es clickeado, counter se incrementa y su cambio se refleja inmediatamente en la interfaz.

### ¿Cómo manejar eventos complejos como formularios?
La gestión de formularios puede parecer complicada, pero se puede simplificar este proceso a través de eventos y modificadores.

1. Evitar el comportamiento por defecto: Utilizar **event.preventDefault()** para interceptar y manejar formularios.
````javascript
methods: {
  submitForm: function(event) {
    event.preventDefault();
    console.log('form submitted');
  }
}
````
2. Modificadores de Vue.js: introducir modificadores como prevent o stop para simplificar el control de eventos.
````html
<form v-on:submit.prevent="submitForm">
  <!-- campos del formulario -->
</form>
````
Estos modificadores permiten gestionar eventos de forma clara y directa, mejorando la legibilidad y el mantenimiento del código.

### ¿Cómo utilizar eventos de teclado y otros?
Vue.js soporta una variedad de eventos, desde interacciones con el mouse hasta teclas específicas.

* Eventos de teclado: Se puede escuchar eventos como keyup y realizar acciones en consecuencia.
````html
<input v-on:keyup="onKeyUp">
````
* Eventos combinados con modificadores: permite una escucha más precisa y directa con modificadores específicos.
````html
<input v-on:keyup.enter="onEnterKey">
````
Estos manejos favorecen la creación de aplicaciones aún más interactivas y personalizadas.

---

