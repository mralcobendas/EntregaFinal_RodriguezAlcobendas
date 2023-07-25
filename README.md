# PreEntrega3_RodriguezAlcobendas


Link al repo:
https://github.com/mralcobendas/PreEntrega3_RodriguezAlcobendas.git

Link al preview: 
https://mralcobendas.github.io/PreEntrega3_RodriguezAlcobendas/






---------------------------

# Mi Cocina Porá
## El sitio de recetas de cocina del nordeste argentino

Mi Cocina Porá es un sitio sobre cocina del nordeste argentino, producido por Ana María Benítez, una cocinera ficticia, aficionada a la cocina del Paraguay y de la región guaranítica argentina. En su sitio web ella:

- Publica recetas regionales
- Guarda un archivo de recetas que los usuarios pueden consultar
- Permite que los usuarios le hagan consultas sobre recetas específicas

Además, Ana María publica un newsletter semanal con las recetas más recientes al que los usuarios pueden suscribirse desde el footer de la web.

## 5 páginas + Error404
Las 5 páginas requeridas son:
- `Index` la home del sitio
- `Recetas` es el archivo de todas las recetas publicadas en el sitio, incuiría un formulario de búsqueda (no está activo) para que los usuarios puedan encontrar rápidamente el contenido que buscar.
- `Sobre mí` donde Ana María se presenta y explica el propósito de su sitio y las características de la cocina de la región. Disclaimer: el texto es ficticio, escrito por ChatGPT.
- `Consultorio` el formulario con el que los usurios pueden enviar sus consultas a Ana María.
- `Receta` la receta detallaa de **Chipá Guazú** sirve de ejemplo de la apariencia que tendrían todas las recetas cuando se hace clic sobre su imagen o título.
- `Error404`: cuando se hace clic sobre cualquier otra receta que no sea la de Chipá Guazú se puede ver la página de error.


## Uso de Boostrap

Para construir el sitio se utilizaron herramientas BS en los siguientes componentes:

- En la `Nav`, que es responsive con botón hamburguesa y que incluye un buscador para que los usuarios encuentran rápidamente la receta que buscan entre las publicadas en el sitio
- Para crear un `Carousel` de recetas destacadas que se muestra en la parte superior de la homepage.
- Para formar la grilla de recetas de la página `Recetas`, que contiene el Archivo de Recetas

En todos los casos, se modificaron los estilos dados por BS para adaptarlos al diseño y las necesidades del sitio.


## Uso de Grid y Flexbox

Tanto Grid como Flexbox fueron utilizadas también para dar forma a diferentes componentes. 
- `Flexbox` puede verse que se utiliza en la grilla de **Últimas Recetas** del Index. Si bien esta grilla conserva el mismo aspecto que la grilla de la página **Recetas**, está construida utilizando una estrategia diferente.
- En cuanto a `Grid`, su aplicación puede verse en la construcción de la receta de **Chipá Guazú**, a la que se accede haciendo clic desde la receta destacada Chipá Guazú del Carousel o desde la primera figure de la grilla de Últimas recetas de la home o del archivo de recetas de la página Recetas.



## SASS
Los estilos fueron compilados en un archivo main.css la sintaxis de SASS, por ejemplo:

- `@Import` para importar las fuentes de Google y los partials de estilos
- `nesting` en casos como, por ejemplo Grilla >> figure >> image (ver estilo de Index en partial "General content")
- `vars` en el partial de Vars se definen los colores del sitio, fuentes, tamaños y pesos tipográficos
- `mixins` se utiliza para definir las propiedades de los componentes lfex que se repiten a lo largo de todo el sitio
- `extend` se aprovecha para definir el estilo de algunos botones (ver partial "Forms")


## SEO

Tanto el Index como las otras páginas cuentan con Title, robots, keywords y metadescription. Todas las imágenes tienen texto alternativo.

## Animaciones

En el partial **Animations** se define una animación del isotipo del sitio que aparece en la página de Error404. Además, los botones de las demás páginas muestran con el hover una transición (que está puesta más para ejercitar el recurso que por criterio estético o de usabilidad)


## Otros requerimientos

- El sitio es responsive para tablet y mobile.
- Las imágenes están optimizadas, al tamaño y en formato webp
- Se utilizaron etiquetas semánticas