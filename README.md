# 🛒 Catálogo digital con carrito y pedido por WhatsApp

Catálogo de productos en una sola página web. El cliente elige lo que quiere, lo añade al carrito, llena sus datos y envía el pedido completo por WhatsApp con un toque.

**Ver el catálogo:** https://y2208.github.io/catalogo-demo/

---

## ✨ Qué hace

- Muestra los productos con foto, descripción y precio en USD.
- Filtros por categoría (Energía solar, Climatización, Refrigeración, Lavadoras, Televisores y Cocinas).
- **Carrito de compras:** añadir productos, subir o bajar cantidades, vaciar y ver el total.
- **Formulario de pedido** con nombre, carnet de identidad, teléfono, provincia, dirección, punto de referencia, tipo de pago (Zelle, USD o CUP) y vuelto.
- **Mensaje listo para WhatsApp** con los datos del cliente, cada producto y el total.
- Se ve bien en celular y no necesita instalar nada.

## 🔄 Cómo funciona

1. El cliente abre el enlace del catálogo.
2. Toca **Añadir al carrito** en los productos que le interesan.
3. Abre el carrito, revisa su pedido y toca **Continuar con mis datos**.
4. Llena el formulario. Si falta algún campo, la página le indica cuál.
5. Toca **Enviar pedido por WhatsApp**. Si WhatsApp no se abre solo, aparece el botón verde **Abrir WhatsApp con mi pedido**.
6. El vendedor recibe un solo mensaje con todo.

## 📁 Archivos

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | Todo el catálogo: diseño, productos, fotos, carrito y formulario |
| `README.md` | Este documento |

La página es un único archivo `index.html`. No usa servidor ni base de datos, y las fotos van incluidas dentro del mismo archivo.

## ⚙️ Configuración

Dentro de `index.html`, cerca del final, hay una variable con el número de WhatsApp que recibe los pedidos:

```js
var WA="5350000000";
```

Se escribe con código de país, sin `+` ni espacios. Por ejemplo, un número de Cuba empieza con `53`.

## 🚀 Publicar con GitHub Pages

1. Sube `index.html` a la raíz del repositorio.
2. Ve a **Settings → Pages**.
3. En **Source** elige **Deploy from a branch**, rama **main** y carpeta **/(root)**.
4. Toca **Save** y espera de 1 a 3 minutos.
5. El enlace queda así: `https://Y2208.github.io/catalogo-demo/`

Para tener varios catálogos, crea una carpeta por cliente con su propio `index.html` dentro, por ejemplo `cliente1/index.html`.

## 🧪 Probar un pedido

1. Abre el enlace publicado en el celular.
2. Añade dos o tres productos y completa el formulario con datos de prueba.
3. Comprueba que el mensaje llega a tu WhatsApp con los datos y el total correctos.

## 🔒 Privacidad

- La página **no guarda ningún dato**. Lo que escribe el cliente solo viaja en el mensaje de WhatsApp hacia el vendedor.
- El carnet de identidad es un dato sensible. Conviene activar la verificación en dos pasos en WhatsApp y no reenviar esos chats.
- Este repositorio es público: cualquiera puede ver el catálogo y el número de WhatsApp configurado.

## 📝 Notas

- Los precios y la disponibilidad pueden cambiar. Para actualizar un precio o un producto hay que modificar la lista de productos dentro de `index.html`.
- Los precios incluyen el transporte.
