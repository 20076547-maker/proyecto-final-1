# proyecto-final-1
✨ DOCUMENTACIÓN DEL PROYECTO
TRUE BEAUTY SALÓN & SPA
1. ¿Qué significa el nombre True Beauty?

True Beauty es una expresión en inglés que significa «Belleza Verdadera».

El nombre representa la filosofía del salón de belleza: resaltar la belleza natural de cada persona mediante servicios profesionales, tratamientos estéticos y productos de calidad.

True: verdadero o auténtico.
Beauty: belleza.

La marca busca transmitir elegancia, confianza, bienestar y cuidado personal.

Eslogan: «Realza tu verdadera esencia».

2. Descripción general del proyecto

True Beauty Salón & Spa es un sitio web diseñado para promocionar los servicios y productos de un salón de belleza.

La página permite a los visitantes conocer el negocio, consultar su catálogo, visualizar promociones, revisar métodos de pago, consultar información de contacto y realizar compras mediante un carrito interactivo.

También incorpora un apartado de inventario para controlar las existencias de los productos y una función para generar e imprimir recibos de compra.

El proyecto está desarrollado utilizando HTML5, Tailwind CSS y JavaScript.

3. Objetivos del proyecto
Objetivo general

Desarrollar una página web moderna, atractiva y funcional que permita presentar los servicios y productos de True Beauty Salón & Spa, facilitando la interacción con los clientes y la administración básica de las compras y el inventario.

Objetivos específicos
Presentar información general del salón.
Mostrar un catálogo de servicios y productos.
Facilitar la selección de productos mediante un carrito.
Permitir la consulta y modificación del inventario.
Mostrar información sobre transferencias bancarias.
Generar recibos de compra imprimibles.
Facilitar la comunicación con los clientes.
Adaptar el diseño a computadoras, tablets y teléfonos móviles.
4. Estructura de los archivos del proyecto

El proyecto se encuentra organizado en dos archivos principales:

text
True-Beauty-Salon/
│
├── index.html
│
└── README.md

Descripción de los archivos
Archivo	Descripción
index.html	Contiene toda la estructura HTML, estilos y programación JavaScript de la página.
README.md	Contiene la documentación y explicación del proyecto.

El archivo index.html reúne las tres partes principales del desarrollo web:

HTML: estructura y contenido.
CSS y Tailwind CSS: diseño y presentación visual.
JavaScript: funciones e interactividad.
5. Tecnologías utilizadas
Tecnología	Función dentro del proyecto
HTML5	Estructura de la página.
CSS3	Estilos personalizados y configuración de impresión.
Tailwind CSS	Diseño visual mediante clases de utilidad.
JavaScript	Funciones interactivas y administración de datos.
Font Awesome	Iconos de navegación, compras y servicios.
Google Fonts	Tipografías Playfair Display y Poppins.
YouTube	Reproducción del video promocional.
5.1 HTML5

Se utiliza para crear los elementos principales de la página, como encabezados, secciones, botones, imágenes, tablas, formularios y enlaces.

Ejemplo:

HTML
<header>
    <nav>
        <a href="#inicio">Inicio</a>
        <a href="#nosotros">Nosotros</a>
        <a href="#catalogo">Catálogo</a>
    </nav>
</header>

5.2 Tailwind CSS

Se utiliza para diseñar la página mediante clases que permiten modificar colores, tamaños, espacios, bordes, sombras y distribución de los elementos.

Ejemplo:

HTML
<div class="bg-white p-8 rounded-3xl shadow-sm">
    <h2 class="text-2xl font-bold text-slate-900">
        True Beauty
    </h2>
</div>

5.3 JavaScript

Se utiliza para programar las funcionalidades de la página, como el carrito de compras, los filtros del catálogo, la actualización del inventario y la generación de recibos.

Ejemplo:

javascript
function toggleCart() {
    const drawer = document.getElementById('cart-drawer');
    drawer.classList.toggle('hidden');
}

6. Estructura principal de la página web

La página está dividida en diferentes secciones que permiten organizar la información y facilitar la navegación.

6.1 Barra de notificaciones

Es la primera sección que aparece en la parte superior de la página.

Su función es mostrar anuncios importantes para los clientes, como promociones, citas y métodos de pago.

Código:

HTML
<div class="bg-slate-900 text-brand-100
text-xs sm:text-sm py-2 px-4 text-center">

    ✨ ¡Agenda tu cita hoy o adquiere
    tus productos favoritos! ✨

</div>

6.2 Encabezado y menú de navegación

El encabezado contiene el logotipo, el nombre del salón, los enlaces de navegación y el acceso al carrito de compras.

Código:

HTML
<header class="sticky top-0 z-40
bg-white/95 backdrop-blur-md shadow-sm">

    <div class="max-w-7xl mx-auto
    px-4 h-20 flex items-center
    justify-between">

        <!-- Logotipo y nombre -->
        <a href="#" class="flex items-center gap-3">

            <div class="w-11 h-11 rounded-full
            bg-gradient-to-tr from-brand-600
            to-brand-400">

                <i class="fa-solid fa-spa"></i>

            </div>

            <div>
                <span>True Beauty</span>
                <span>Salón & Spa</span>
            </div>

        </a>

    </div>

</header>

Elementos del encabezado
Logotipo circular con icono de spa.
Nombre comercial True Beauty.
Identificación del salón como Salón & Spa.
Menú de navegación.
Botón de carrito.
Contador de productos seleccionados.
Menú adaptable para dispositivos móviles.
6.3 Sección de inicio (Hero)

Es la primera presentación visual del negocio.

Contiene un mensaje de bienvenida, una descripción del salón, botones de acceso y una imagen representativa.

Identificador:

HTML
<section id="inicio">


Su función es captar la atención de los visitantes y dirigirlos hacia el catálogo o los métodos de pago.

6.4 Sección Nosotros

Contiene la misión y visión de True Beauty Salón & Spa.

Identificador:

HTML
<section id="nosotros">


Se divide en dos apartados:

Misión: brindar servicios de belleza y bienestar de calidad mediante atención personalizada.
Visión: convertirse en un salón reconocido por su innovación, elegancia y satisfacción de los clientes.
6.5 Catálogo de servicios y productos

Permite visualizar los servicios y productos disponibles.

Identificador:

HTML
<section id="catalogo">


Incluye:

Corte estilizado y brushing.
Balayage o rayitos premium.
Maquillaje profesional.
Manicure y pedicure.
Shampoo revitalizante.
Mascarilla reparadora.
Aceite protector térmico.
Depilación láser.

También incorpora filtros para mostrar todos los artículos, únicamente servicios o únicamente productos.

Código:

HTML
<button onclick="filterCatalog('all')">
    Todos
</button>

<button onclick="filterCatalog('Servicio')">
    Servicios
</button>

<button onclick="filterCatalog('Producto')">
    Productos
</button>

<div id="catalog-grid"></div>

6.6 Video promocional

Identificador:

HTML
<section id="video">


Esta sección contiene un video integrado desde YouTube para promocionar los servicios y mostrar la experiencia que ofrece el salón.

6.7 Métodos de pago y transferencias

Identificador:

HTML
<section id="transferencias">


Presenta los datos de las cuentas bancarias y las opciones de pago.

Incluye:

Banco Cuscatlán.
Banco Agrícola.
Chivo / Pago Móvil.

También cuenta con botones que permiten copiar los números de cuenta.

6.8 Tabla de inventario

Identificador:

HTML
<section id="inventario">


Permite consultar y modificar las existencias de productos e insumos.

La tabla contiene:

Código del producto.
Nombre del producto.
Categoría.
Precio unitario.
Stock actual.
Estado del inventario.
Acciones para aumentar o disminuir el stock.

Identificadores utilizados:

HTML
id="inventory-count"

id="inventory-table-body"


Estos elementos permiten que JavaScript actualice la cantidad total de artículos y el contenido de la tabla.

6.9 Ubicación y contacto

Identificador:

HTML
<section id="contacto">


Muestra los datos de ubicación del salón, horarios, teléfonos y redes sociales.

Incluye enlaces a:

Instagram.
Facebook.
TikTok.
WhatsApp.
Correo electrónico.
6.10 Pie de página (Footer)

Es la última sección de la página.

Contiene el nombre del negocio, derechos reservados y enlaces de navegación.

Código:

HTML
<footer class="bg-slate-950
text-slate-400 py-12">

    <span>True Beauty Salón & Spa</span>

    <p>
        © 2026 True Beauty Salón & Spa.
        Todos los derechos reservados.
    </p>

</footer>

7. Logotipo e identidad visual

El logotipo está representado mediante un icono de spa dentro de un círculo con un degradado de colores de la marca.

Código:

HTML
<div class="w-11 h-11 rounded-full
bg-gradient-to-tr from-brand-600
to-brand-400 flex items-center
justify-center text-white shadow-md">

    <i class="fa-solid fa-spa text-lg"></i>

</div>

Tipografías

Se utilizan dos fuentes de Google Fonts:

Playfair Display: utilizada principalmente en títulos y elementos que requieren una apariencia elegante.
Poppins: utilizada en párrafos, botones, navegación y textos generales.
Paleta de colores

Color principal: Brand

Nivel	Código
50	#fdf8f6
100	#fbe8e6
200	#f5d3d0
300	#ecb1ac
400	#e0847d
500	#d16056
600	#bc483e
700	#9e3b33
800	#82342e
900	#6c2f2a

Color secundario: Gold

Nivel	Código
50	#fcfae1
100	#f7f1b4
200	#f1e57c
300	#ebd843
400	#e4cd1b
500	#cbaf0e
600	#a28a0a
700	#7e6b0a
800	#68570c
900	#58490f
Configuración de colores en Tailwind CSS
javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                brand: {
                    50: '#fdf8f6',
                    100: '#fbe8e6',
                    200: '#f5d3d0',
                    300: '#ecb1ac',
                    400: '#e0847d',
                    500: '#d16056',
                    600: '#bc483e',
                    700: '#9e3b33',
                    800: '#82342e',
                    900: '#6c2f2a'
                },
                gold: {
                    50: '#fcfae1',
                    100: '#f7f1b4',
                    200: '#f1e57c',
                    300: '#ebd843',
                    400: '#e4cd1b',
                    500: '#cbaf0e',
                    600: '#a28a0a',
                    700: '#7e6b0a',
                    800: '#68570c',
                    900: '#58490f'
                }
            }
        }
    }
}


Nota técnica: En el código HTML original se configura la paleta Gold, mientras que también se utilizan clases brand-*. Para que ambas paletas funcionen con la configuración mostrada, hay que agregar Brand como en el ejemplo anterior.

8. Clases principales utilizadas

Las clases son instrucciones que permiten establecer la apariencia de cada elemento HTML.

El proyecto utiliza principalmente clases de Tailwind CSS.

8.1 Clases de colores
Clase	Función
bg-white	Fondo blanco.
bg-brand-600	Fondo con el color principal.
bg-slate-900	Fondo gris oscuro.
text-white	Texto blanco.
text-slate-600	Texto gris.
text-brand-600	Texto con el color principal.
border-brand-100	Borde con color de marca.
8.2 Clases de distribución
Clase	Función
flex	Activa el modelo Flexbox.
grid	Activa el sistema Grid.
items-center	Centra elementos verticalmente.
justify-between	Distribuye elementos en los extremos.
justify-center	Centra elementos horizontalmente.
flex-col	Organiza elementos en columna.
gap-4	Agrega separación entre elementos.
grid-cols-1	Organiza el contenido en una columna.
md:grid-cols-2	Organiza el contenido en dos columnas desde pantallas medianas.
8.3 Clases de dimensiones y espacios
Clase	Función
w-full	Ocupa todo el ancho disponible.
h-20	Establece una altura.
max-w-7xl	Limita el ancho máximo.
mx-auto	Centra horizontalmente.
p-8	Agrega espacio interior.
px-4	Espacio horizontal interior.
py-20	Espacio vertical interior.
mt-4	Margen superior.
mb-6	Margen inferior.
8.4 Clases de diseño y efectos
Clase	Función
rounded-full	Bordes completamente redondeados.
rounded-3xl	Bordes redondeados amplios.
shadow-sm	Sombra pequeña.
shadow-xl	Sombra pronunciada.
hover:bg-brand-700	Cambia el fondo al pasar el cursor.
transition	Suaviza los cambios visuales.
overflow-hidden	Oculta el contenido que sobresale.
font-bold	Aplica negrita.
text-center	Centra el texto.
uppercase	Convierte el texto a mayúsculas.
8.5 Clases responsivas

Se utilizan prefijos para adaptar el diseño a diferentes tamaños de pantalla.

Prefijo	Uso
sm:	Pantallas pequeñas y superiores.
md:	Pantallas medianas y superiores.
lg:	Pantallas grandes y superiores.

Ejemplo:

HTML
<div class="grid grid-cols-1
sm:grid-cols-2 lg:grid-cols-3">

</div>


Esto permite mostrar una columna en dispositivos pequeños, dos en pantallas pequeñas más amplias y tres en pantallas grandes.

9. Identificadores (ID) principales

Los identificadores permiten localizar elementos específicos del documento HTML mediante JavaScript y también sirven como destinos de los enlaces de navegación.

9.1 Identificadores de las secciones
ID	Elemento
inicio	Página principal.
nosotros	Misión y visión.
catalogo	Catálogo de servicios y productos.
video	Video promocional.
transferencias	Métodos de pago.
inventario	Tabla de inventario.
contacto	Ubicación y contacto.
9.2 Identificadores del carrito
ID	Función
cart-drawer	Panel lateral del carrito.
cart-backdrop	Fondo oscuro del carrito.
cart-counter	Contador de artículos.
cart-item-count-label	Cantidad de artículos en el panel.
cart-items-container	Contenedor de productos seleccionados.
cart-subtotal	Subtotal de compra.
cart-tax	Impuesto calculado.
cart-total	Total de compra.
checkout-ref	Referencia de transferencia.
checkout-btn	Botón para generar el recibo.
9.3 Identificadores del recibo
ID	Función
receipt-modal	Ventana del recibo.
printable-receipt	Área imprimible.
receipt-invoice-no	Número del recibo.
receipt-date	Fecha de compra.
receipt-payment-method	Método de pago.
receipt-items-body	Tabla de artículos comprados.
receipt-subtotal-val	Subtotal del recibo.
receipt-tax-val	Impuesto del recibo.
receipt-total-val	Total pagado.
receipt-transfer-note-box	Área de referencia bancaria.
receipt-transfer-ref	Número de referencia.
9.4 Identificadores del inventario
ID	Función
inventory-count	Total de productos registrados.
inventory-table-body	Contenido de la tabla.
inv-stock-${item.id}	Identifica la existencia de cada producto.
9.5 Identificadores de navegación
ID	Función
mobile-menu	Menú de navegación móvil.
mobile-menu-icon	Icono del menú móvil.
btn-cat-all	Filtro de todos los artículos.
btn-cat-Servicio	Filtro de servicios.
btn-cat-Producto	Filtro de productos.
10. Funciones principales de JavaScript

JavaScript permite que la página tenga funcionalidades dinámicas e interactivas.

A continuación se describen las funciones principales.

10.1 toggleMobileMenu()

Abre y cierra el menú de navegación para dispositivos móviles.

javascript
function toggleMobileMenu() {
    const menu = document.getElementById('mobile-menu');

    menu.classList.toggle('hidden');
}

10.2 filterCatalog(category)

Permite filtrar los artículos del catálogo según su categoría.

Recibe como parámetro:

all: todos los artículos.
Servicio: solamente servicios.
Producto: solamente productos.
10.3 renderCatalog(filterCategory)

Genera dinámicamente las tarjetas del catálogo con imágenes, nombres, precios, descripciones y botones para agregar artículos.

10.4 renderInventoryTable()

Construye la tabla de inventario y muestra la información de los productos registrados.

10.5 updateStock(id, change)

Permite aumentar o disminuir la cantidad disponible de un producto.

Parámetros:

id: identificador del producto.
change: cantidad que se suma o resta.
10.6 toggleCart()

Abre o cierra el panel lateral del carrito de compras.

10.7 addToCart(id)

Agrega un producto o servicio al carrito.

Si el artículo ya existe, aumenta su cantidad.

10.8 updateCartQuantity(id, change)

Permite modificar la cantidad de un artículo dentro del carrito.

10.9 removeFromCart(id)

Elimina un producto o servicio seleccionado.

10.10 clearCart()

Vacía completamente el carrito de compras.

10.11 updateCartUI()

Actualiza visualmente el contenido del carrito, la cantidad de artículos, el subtotal, los impuestos y el total.

10.12 openReceiptModal()

Genera el recibo de compra utilizando los productos seleccionados y calcula los valores correspondientes.

También muestra el número de recibo, la fecha y la referencia de transferencia cuando existe.

10.13 closeReceiptModal()

Cierra la ventana del recibo de compra.

10.14 printReceipt()

Permite imprimir el recibo utilizando la función de impresión del navegador.

javascript
function printReceipt() {
    window.print();
}

10.15 copyToClipboard(text)

Copia al portapapeles el número de cuenta bancaria seleccionado.

javascript
function copyToClipboard(text) {
    navigator.clipboard.writeText(text);
}

11. Datos del catálogo

Los productos y servicios están almacenados en un arreglo de objetos llamado catalogItems.

Cada elemento contiene información específica.

Ejemplo:

javascript
const catalogItems = [
    {
        id: 1,
        name: "Corte Estilizado & Brushing",
        category: "Servicio",
        price: 35.00,
        image: "imagen-del-producto.jpg",
        description: "Corte de cabello personalizado.",
        stock: 15
    }
];

Descripción de sus propiedades
Propiedad	Descripción
id	Número de identificación.
name	Nombre del producto o servicio.
category	Categoría del artículo.
price	Precio de venta.
image	Dirección de la imagen.
description	Descripción del artículo.
stock	Cantidad disponible.
12. Cálculo de compras e impuestos

El sistema calcula automáticamente el subtotal, el IVA y el total de la compra.

La tasa configurada en el código es del 13%.

Ejemplo:

javascript
const subtotal = 100.00;

const tax = subtotal * 0.13;

const total = subtotal + tax;


Resultado:

Concepto	Valor
Subtotal	$100.00
IVA (13%)	$13.00
Total	$113.00
13. Diseño adaptable (Responsive Design)

La página utiliza clases responsivas de Tailwind CSS para adaptar su contenido a diferentes dispositivos.

Se utilizan principalmente:

sm: para pantallas pequeñas y superiores.
md: para pantallas medianas y superiores.
lg: para pantallas grandes y superiores.

También incluye un menú móvil que permite acceder a las diferentes secciones desde teléfonos y tablets.

14. Estilos especiales para impresión

El proyecto incorpora una regla CSS para imprimir únicamente el recibo de compra.

Código:

css
@media print {

    body * {
        visibility: hidden;
    }

    #printable-receipt,
    #printable-receipt * {
        visibility: visible;
    }

    #printable-receipt {
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        background: white;
    }

    .no-print {
        display: none !important;
    }
}


Esta configuración oculta el resto de la página y muestra únicamente el contenido del recibo al momento de imprimir.

15. Instalación y ejecución

Para ejecutar el proyecto localmente se deben seguir estos pasos:

Paso 1. Descargar el proyecto y guardarlo en una carpeta.

Paso 2. Abrir la carpeta con Visual Studio Code.

Paso 3. Verificar que exista el archivo index.html.

Paso 4. Abrir el archivo utilizando un navegador web o la extensión Live Server.

Paso 5. Navegar por las diferentes secciones y probar las funcionalidades.

No es necesario instalar una base de datos para ejecutar la versión actual.

16. Limitaciones actuales del proyecto

El sistema funciona como una aplicación frontend de demostración.

Actualmente:

Los datos del catálogo están almacenados en JavaScript.
El inventario no tiene almacenamiento permanente.
El carrito no está conectado a una base de datos.
No existe un sistema de usuarios.
No se encuentra integrada una pasarela de pago.
Los recibos son comprobantes internos imprimibles, no documentos fiscales electrónicos.
Los datos bancarios y comerciales deben verificarse antes de utilizarlos en un negocio real.
17. Mejoras futuras

Se pueden incorporar nuevas funcionalidades para convertir la página en un sistema comercial más completo.

Conectar una base de datos.
Crear un panel administrativo.
Implementar inicio de sesión.
Guardar los cambios del inventario.
Incorporar reservaciones de citas.
Agregar historial de compras.
Integrar métodos de pago electrónicos.
Crear reportes de ventas.
Implementar comprobantes fiscales mediante un sistema autorizado.
18. Conclusión

El proyecto True Beauty Salón & Spa representa una solución digital para la presentación y administración básica de un salón de belleza.

Mediante HTML5 se organiza la información, Tailwind CSS proporciona una presentación visual moderna y JavaScript permite implementar funcionalidades como el catálogo, el inventario, el carrito de compras y la generación de recibos.

El desarrollo busca ofrecer una experiencia agradable para los clientes, facilitar la consulta de los servicios y productos y fortalecer la presencia digital del negocio.

19. Información del proyecto
Campo	Información
Nombre del proyecto	True Beauty Salón & Spa
Significado	Belleza Verdadera
Tipo de proyecto	Página web comercial
Área	Belleza, estética y cuidado personal
Lenguajes	HTML5, CSS3 y JavaScript
Framework CSS	Tailwind CSS
Año	2026
Archivo principal	index.html
Documentación	README.md

TRUE BEAUTY SALÓN & SPA

«Realza tu verdadera esencia» ✨
