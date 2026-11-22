# Taller 6 – GUIs con Swing y Java2D

Aplicación de escritorio (Swing) para llevar un diario de restaurantes visitados y por visitar.

## Contenido

- `Taller Swing Restaurantes Esqueleto/` – proyecto Eclipse con la solución.
- `diagrama_clases.png` – diagrama de clases de la aplicación completa (superclases, interfaces y asociaciones).

## Cómo ejecutar

La aplicación carga las imágenes con rutas relativas (`./imagenes/...`), así que **debe ejecutarse con la carpeta del proyecto como directorio de trabajo**. Requiere Java 11 o superior.

### Desde Eclipse

1. `File > Import > General > Existing Projects into Workspace` y seleccionar la carpeta `Taller Swing Restaurantes Esqueleto`.
2. Abrir `src/uniandes/dpoo/swing/interfaz/principal/VentanaPrincipal.java`.
3. `Run As > Java Application` (Eclipse usa la carpeta del proyecto como directorio de trabajo por defecto).

### Desde la terminal

```sh
cd "Taller Swing Restaurantes Esqueleto"
javac -encoding UTF-8 -d bin $(find src -name "*.java")
java -cp bin uniandes.dpoo.swing.interfaz.principal.VentanaPrincipal
```

## Uso

- **Ventana principal:** lista de restaurantes; al seleccionar uno se muestran su nombre, calificación (estrellas) y si fue visitado.
- **Nuevo:** abre la ventana para agregar un restaurante. Se hace click sobre el mapa para marcar su ubicación, se ingresan nombre, calificación y si fue visitado, y se presiona *Agregar*.
- **Ver todos:** abre el mapa con todos los restaurantes marcados; los radio buttons permiten ver todos o solo los visitados.
