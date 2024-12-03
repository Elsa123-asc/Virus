### Manual Básico de jQuery

#### ¿Qué es jQuery?
jQuery es una herramienta que simplifica el uso de JavaScript para crear interactividad en páginas web. Con jQuery, puedes manipular elementos de una página web de forma sencilla y eficiente.

---

### **Primeros pasos con jQuery**

#### **1. Cargar las librerías de jQuery**
Antes de usar jQuery en tu página, es necesario incluir su librería. Esto se hace añadiendo el siguiente script en el archivo HTML:

```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
```

Este script asegura que tienes acceso a las funciones y características de jQuery.

#### **2. Crear un archivo para tu código**
Tu código jQuery debe estar dentro de otro script, que tendrá siempre la misma estructura base:

```html
<script>
jQuery(document).ready(function() {
    // Aquí va tu código
});
</script>
```

Esta estructura significa que el código dentro de `jQuery(document).ready` se ejecutará una vez que la página web haya terminado de cargar. De esta forma, garantizamos que los elementos de la página estén disponibles para ser manipulados.

---

### **Cómo escribir código jQuery**

El formato básico de cualquier acción en jQuery es el siguiente:

```javascript
$(elemento).accion();
```

#### **Definir elementos**
Para indicar a qué parte de tu página quieres aplicar una acción, puedes definir el elemento de tres maneras:

1. **Por tipo de elemento HTML**  
   Selecciona todos los elementos de un tipo específico, como todos los párrafos `<p>` o todas las imágenes `<img>`:

   ```javascript
   $("nombre")
   ```
   **Ejemplo:**  
   ```javascript
   $("p").hide(); // Oculta todos los párrafos
   ```

2. **Por identificador (id)**  
   Selecciona un único elemento que tenga un identificador específico:

   ```javascript
   $("#nombre")
   ```
   **Ejemplo:**  
   ```javascript
   $("#titulo").show(); // Muestra el elemento con id="titulo"
   ```

3. **Por clase**  
   Selecciona todos los elementos que compartan una clase:

   ```javascript
   $(".nombre")
   ```
   **Ejemplo:**  
   ```javascript
   $(".boton").css("color", "red"); // Cambia el color del texto de todos los elementos con clase="boton"
   ```

---

### **Acciones comunes en jQuery**
Algunas acciones básicas que puedes usar en jQuery:

- **Ocultar elementos:**  
  ```javascript
  $(elemento).hide();
  ```

- **Mostrar elementos:**  
  ```javascript
  $(elemento).show();
  ```

- **Cambiar propiedades CSS:**  
  ```javascript
  $(elemento).css("propiedad", "valor");
  ```

- **Añadir texto o contenido:**  
  ```javascript
  $(elemento).text("Nuevo texto");
  $(elemento).html("<strong>Texto en negrita</strong>");
  ```

- **Añadir o eliminar clases:**  
  ```javascript
  $(elemento).addClass("nuevaClase");
  $(elemento).removeClass("claseExistente");
  ```

---

### **Tu primer ejemplo práctico**
1. Abre un archivo HTML.
2. Copia y pega el siguiente código para probar tu primer script en jQuery:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejemplo jQuery</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
</head>
<body>
    <h1 id="titulo">¡Hola, mundo!</h1>
    <button id="boton">Haz clic aquí</button>

    <script>
    jQuery(document).ready(function() {
        $("#boton").click(function() {
            $("#titulo").hide();
        });
    });
    </script>
</body>
</html>
```

3. Abre el archivo en tu navegador. Cuando hagas clic en el botón, el título desaparecerá.

---

### **Resumen**
1. Incluye siempre la librería de jQuery.
2. Usa la estructura básica para tu código.
3. Define elementos por nombre, id o clase.
4. Aplica acciones usando el formato `$(elemento).accion();`.

¡Listo! Ahora tienes lo básico para empezar a trabajar con jQuery. 🎉
