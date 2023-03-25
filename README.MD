# eCommerce backend

Proyecto final del curso de backend con nodejs en Coderhouse.



## ⭐ Acerca del proyecto


Proyecto backend donde se implementa un API e-commerce para poder vender productos.

## 📝 Descripción

---

- API para manejar productos.
- API para manejar usuarios.
- API para manejar autenticación (login y uso de JWT)
- API para manejar carrito de compras
- Uso de servicios de gmail, WhatsApp y storage para imágenes.
  - gmail para confirmar registro de usuario y venta de carrito.
  - WhatsApp para confirmar venta de carrito.
  - storage para subir photo del usuario.
- MongoDB para persistir la data en producción y la opción de utilizar en memoria para desarrollo.
- Poder habilitar el modo CLUSTER mediante variable de entorno.
- Implementar registro de logs V1 con winston y morgan.
- Trabajar con dependencias typescript y ts-node-dev en vez de Webpack.
- Implementar el proyecto en TypeScript.
- Implementar el proyecto en capas.
  - routes: capa de rutas
  - controllers: capa de controladores
  - business: capa de negocio
  - persistence: capa de persistencia con implementación de repository, dto y dao.

## Prueba todas las opciones de la api

---

- API de prueba temporal en:/api/products

  - Usuario admin para probar todos los endpoints sin restricciones:


- La documentación en Swagger está en proceso: api/docs


## 📦 Estructura de carpetas

---

```
├── build
├── logs
├── src
│   ├── business
│   ├── controllers
│   ├── middleware
│   │   ├── errors
│   │   ├── routes
│   │   ├── security
│   │   └── validators
│   ├── persistence
│   │   ├── dao
│   │   │   ├── productDao
│   │   │   ├── shoppingCartDao
│   │   │   └── userDao
│   │   ├── dto
│   │   └── repository
│   ├── routes
│   ├── services
│   │   ├── email
│   │   ├── storage
│   │   └── whatsapp
│   ├── store
│   │   ├── daos
│   │   ├── FileSystem
│   │   ├── firebase
│   │   ├── mongoDb
│   │   │   └── models
│   │   └── types
│   └── types
└── storage

```

## 🛠️ Técnologias y recursos

---

- Node.js
- Express
- Typescript
- MongoDB
- Passport JWT
- Mongoose
- Bcrypt
- Dotenv
- Nodemailer
- Twilio
- (más detalle en el package.json)


## 🛠️ Available Scripts

---

### `npm run dev`

Corre el proyecto en modo desarrollo

### `npm run clean`

Elimina el build generado del proyecto

### `npm run build`

Construye el build del proyecto

### `npm run start`

Corre el build generado del proyecto en modo producción

## 🙌 Mis notas para seguir mejorando el proyecto

---

- Actualizar la documentación con swagger (Investigar como implementar la documentación por comentarios)
- Investigar como extender las propiedades del Request de Express con TypeScript para no usar req["newProperty"]
- Investigar estrategias de subida de archivos para que se cargue con previa validación de negocio. (Como alternativa eliminar el recurso si el registro fallo por validación de negocio)
- Mejorar la funcionalidad de vender el carrito de compras (Manejar cantidad por producto y actualización del stock)

<br>
<br>
<br>