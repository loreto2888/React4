

## Hito 4 - Pizzería Mamá Mía 🍕

¡Bienvenido/a al proyecto **Pizzería Mamá Mía**!

Este proyecto corresponde al Hito 4 del bootcamp Desafío Latam. Es una aplicación web desarrollada con React y Vite que simula el sitio de una pizzería, permitiendo:

- Autenticación de usuario (login).
- Listado de pizzas con imágenes, nombres, precios e ingredientes.
- Agregar pizzas al carrito y modificar cantidades.
- Realizar la compra y vaciar el carrito.
- Navegación entre páginas mediante un Navbar.
- Componentes reutilizables (Header, Footer, CardPizza, etc).
- Estilos modernos y responsivos en CSS.

---


## Características principales

- Login y registro de usuario.
- Listado de pizzas con imágenes, nombres, precios e ingredientes.
- Carrito de compras con suma total y opción de pagar.
- Navegación entre Home, Login, Register y Carrito.
- Componentes reutilizables y contexto para el carrito.
- Estilos modernos y responsivos.


## Estructura del proyecto

```
├── public/
│   └── vite.svg
├── src/
│   ├── App.jsx
│   ├── main.jsx
│   ├── styles.css
│   ├── components/
│   │   ├── CardPizza.jsx
│   │   ├── Cart.jsx
│   │   ├── Footer.jsx
│   │   ├── Header.jsx
│   │   ├── Home.jsx
│   │   ├── Login.jsx
│   │   ├── Navbar.jsx
│   │   ├── Register.jsx
│   ├── context/
│   │   └── CartContext.jsx
│   └── utils/
│       ├── format.js
│       └── pizzas.js
├── index.html
├── package.json
├── vite.config.js
├── eslint.config.js
└── README.md
```


## Instalación y ejecución

1. **Clona el repositorio:**
	```bash
	git clone <url-del-repositorio>
	cd Hito1_pizzeriamamamia_JohannaBarrientos
	```
2. **Instala las dependencias:**
	```bash
	npm install
	```
3. **Inicia la aplicación en modo desarrollo:**
	```bash
	npm run dev
	```
4. Abre tu navegador en [http://localhost:5173](http://localhost:5173) (o el puerto que indique Vite) para ver la app.


## ¿Cómo usar la app?

1. Ingresa con tu email y contraseña en la página de Login.
2. Explora las pizzas disponibles en la página principal.
3. Agrega las pizzas que desees al carrito.
4. Accede al carrito para modificar cantidades o realizar la compra.
5. Al pagar, el carrito se vacía y puedes seguir comprando.

- `npm run dev` — Inicia el servidor de desarrollo.
- `npm run build` — Genera la versión de producción.
- `npm run preview` — Previsualiza la app en modo producción.

## Tecnologías utilizadas

- [React](https://react.dev/)
- [Vite](https://vitejs.dev/)
- [JavaScript](https://developer.mozilla.org/es/docs/Web/JavaScript)
- [CSS](https://developer.mozilla.org/es/docs/Web/CSS)


## Autor

- Johanna Barrientos
- Desafío Latam — Hito 4

---

¡Gracias por visitar este proyecto! Si tienes sugerencias o encuentras algún error, no dudes en abrir un issue o hacer un pull request.


campos que estoy ocupando en Home.jsx
{
    id: 1,
    nombre: "Margarita",
    precio: 8000,
  imagen: "img/Margarita.jpg",
    ingredientes: ["Queso mozzarella", "Tomate", "Albahaca"]
  },

campos de pizzabackend.json
{
    "desc": "La pizza napolitana, de masa tierna y delgada pero bordes altos, es la versión propia de la cocina napolitana de la pizza redonda. El término pizza napoletana, por su importancia histórica o regional, se emplea en algunas zonas como sinónimo de pizza tonda.",
    "id": "p001",
    "img": "https://firebasestorage.googleapis.com/v0/b/apis-varias-mias.appspot.com/o/pizzeria%2Fpizza-1239077_640_cl.jpg?alt=media&token=6a9a33da-5c00-49d4-9080-784dcc87ec2c",
    "ingredients": ["mozzarella", "tomates", "jamón", "orégano"],
    "name": "napolitana",
    "price": 5950
  },

  campo original y campo nuevo

id={pizza.id}  ok
nombre={pizza.nombre}  name
precio={pizza.precio}  price
ingredientes={pizza.ingredientes} ingredients
imagen={pizza.imagen}  img
onAddToCart={() => addToCart(pizza)}