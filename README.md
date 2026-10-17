# Tienda de Productos y Servicios

Tienda de Productos y Servicios es un proyecto desarrollado en **Java** que modela la gestión de una tienda mediante programación orientada a objetos. Permite administrar productos, servicios, clientes, vendedores y ventas, así como controlar el stock de los productos y calcular el importe total de cada venta.

```text
Estado: proyecto académico con funcionalidades implementadas y pruebas unitarias.
```

## Índice
* [Funcionalidades principales](#funcionalidades-principales)
* [Objetivo](#objetivo)
* [Estructura del proyecto](#estructura-del-proyecto)
* [🛠 Lenguajes y tecnologías](#-lenguajes-y-tecnologías)
* [Cómo ejecutar](#cómo-ejecutar)
* [Autora](#autora)

## Funcionalidades principales
- Registrar productos en el inventario e indicar su stock.
- Registrar servicios con precio, fecha de inicio y fecha de finalización.
- Registrar y consultar clientes y vendedores.
- Crear ventas y asociarlas con un cliente y un vendedor.
- Agregar productos y servicios a una venta.
- Descontar automáticamente las unidades vendidas del stock de productos.
- Lanzar una excepción personalizada cuando no hay stock suficiente.
- Calcular el total de una venta a partir de los ítems y sus cantidades.
- Ejecutar pruebas unitarias para validar el registro de entidades, las ventas y el control de inventario.

## Objetivo
El proyecto se realizó con el objetivo de aplicar los fundamentos de **programación orientada a objetos (POO)** en Java a un caso de negocio: una tienda que comercializa productos y servicios.

Se trabajan conceptos como **clases y objetos, encapsulamiento, interfaces, polimorfismo, colecciones (`HashMap`), manejo de excepciones y pruebas unitarias**.

La interfaz `Vendible` define las operaciones comunes de productos y servicios; la clase `Tienda` concentra la administración de entidades e inventario, y la clase `Venta` agrupa los ítems vendidos y calcula sus importes.

## Estructura del proyecto
Este repositorio contiene **código Java y pruebas unitarias**, no una interfaz gráfica. Por ello, esta sección reemplaza las capturas de pantalla del README de referencia por una descripción de sus componentes.

```text
TiendaProductosYServicios/
├── src/ar/edu/unlam/dominio/
│   ├── Tienda.java
│   ├── Vendible.java
│   ├── Producto.java
│   ├── Servicio.java
│   ├── Cliente.java
│   ├── Vendedor.java
│   ├── Venta.java
│   └── *Exception.java
├── test/ar/edu/unlam/test/
│   └── testTienda.java
├── .project
└── .classpath
```

**Componentes principales:**
- **`Tienda`:** almacena productos, servicios, clientes, vendedores y ventas mediante mapas identificados por código o documento.
- **`Vendible`:** interfaz que comparten `Producto` y `Servicio`.
- **`Producto`:** registra código, nombre, precio y stock.
- **`Servicio`:** registra código, nombre, precio y fechas de inicio y fin.
- **`Venta`:** asocia cliente, vendedor e ítems, y calcula el total.
- **Excepciones personalizadas:** incluyen `StockInsuficienteException` y otras excepciones definidas en el dominio.

## 🛠 Lenguajes y tecnologías
- **Java 18**
- **JUnit 4** para pruebas unitarias
- **Eclipse IDE** (el repositorio incluye archivos de configuración de Eclipse)
- **Programación orientada a objetos (POO)**
- **Java Collections Framework:** `Map` y `HashMap`

## Cómo ejecutar
**Requisitos:**
- Tener instalado **JDK 18** (es la versión configurada en `.classpath`).
- Utilizar **Eclipse IDE** con soporte para Java y JUnit 4.

**1. Clonar el repositorio:**

```bash
git clone https://github.com/Karen-nina/TiendaProductosYServicios.git
```

**2. Importar el proyecto en Eclipse:**
1. Abrir Eclipse.
2. Seleccionar **File → Import → General → Existing Projects into Workspace**.
3. Elegir la carpeta `TiendaProductosYServicios` y finalizar la importación.
4. Comprobar que el proyecto utilice **JavaSE-18** y tenga disponible **JUnit 4** en su *Build Path*.

**3. Ejecutar las pruebas unitarias:**
1. Abrir `test/ar/edu/unlam/test/testTienda.java`.
2. Hacer clic derecho en el archivo.
3. Seleccionar **Run As → JUnit Test**.

Las pruebas incluidas verifican el alta de productos, stock, clientes y vendedores; las ventas de productos y servicios; el cálculo de totales; y el rechazo de ventas cuando el stock es insuficiente.

> **Nota:** El repositorio no incluye una clase `main` ni una aplicación web. Su funcionamiento se comprueba principalmente mediante las pruebas JUnit.

## Autora
- **Karen Nina Coela** — [GitHub](https://github.com/Karen-nina)

---
Si querés explorar el código, podés consultar directamente el [repositorio TiendaProductosYServicios](https://github.com/Karen-nina/TiendaProductosYServicios).
