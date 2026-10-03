# 🍣 Sushi Express - Sistema de Pedidos y Tickets Móvil

Aplicación web progresiva (PWA) optimizada para dispositivos móviles (Android / iOS) diseñada para la gestión de pedidos, tickets de comida, catálogo de platillos (Suchis y Bebidas), e impresión térmica directa.

## 🚀 Características Principales

* **Catálogo Organizado:** Pestañas separadas para **Suchis / Roles** y **Bebidas**, permitiendo agregar o modificar precios y productos fácilmente.
* **Formato de Ticket Térmico / Comandera:** Estructura de impresión optimizada para rollos de 80mm o impresoras portátiles de tickets (`window.print()`).
* **Modo Oscuro / Claro:** Adaptable mediante un botón de alternancia rápida.
* **Historial de Pedidos:** Almacenamiento local (localStorage) para guardar, cargar o reimprimir pedidos previos con folios automáticos (`#ORD-...`).
* **Exportación y Respaldos:** 
  * Exportación de tickets a **Excel (.xlsx)** mediante SheetJS.
  * Envío directo de resumen de pedido vía **WhatsApp**.
  * Respaldo y restauración completa de datos en formato **JSON**.
* **Funcionamiento Offline:** Soporta Service Worker para uso sin conexión a internet.

## 📂 Estructura del Repositorio

```text
├── index.html       # Interfaz principal y lógica de la aplicación
├── manifest.json    # Configuración de PWA
├── sw.js            # Service Worker para caché offline
└── README.md        # Documentación del proyecto
```

## 🛠️ Cómo desplegar en GitHub Pages

1. Sube estos archivos a un repositorio nuevo en GitHub (por ejemplo, `sushi-express`).
2. Ve a la pestaña **Settings** (Configuración) de tu repositorio.
3. En la sección lateral izquierda, haz clic en **Pages**.
4. En **Build and deployment**, selecciona la rama `main` (o `master`) y la carpeta `/ (root)` como fuente (*Branch*).
5. Haz clic en **Save**. En unos segundos, GitHub te proporcionará el enlace público para acceder a tu cotizador/ticketera desde cualquier celular o tablet.
