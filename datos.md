# ¿Qué es un CSV?
CSV (Comma-Separated Values) es un formato de archivo que almacena datos en forma de tabla, donde cada línea representa una fila y los valores están separados por comas (,), aunque también pueden usarse otros delimitadores como punto y coma (;) o tabulaciones.

## Características del formato CSV
- Texto plano: Se puede abrir con cualquier editor de texto.
- Estructura tabular: Similar a una hoja de cálculo (Excel, Google Sheets).
- Delimitador: Generalmente se usa la coma (,), pero puede variar según la configuración regional.
- Encabezado opcional: Puede incluir una primera fila con los nombres de las columnas.
  
## Ejemplo de un archivo CSV
csv
Copiar código
Nombre,Edad,Ciudad
Juan,25,Madrid
Ana,30,Buenos Aires
Luis,22,México
Aquí, cada fila representa una persona, con sus datos separados por comas.

# ¿Cómo funciona?
Los archivos CSV permiten almacenar datos estructurados de manera sencilla y son compatibles con múltiples herramientas, como:

- Excel: Puedes abrir y guardar archivos CSV fácilmente.
- Bases de datos: Se usan para importar/exportar datos.
- Lenguajes de programación: Python, R, JavaScript, y otros pueden leer y escribir archivos CSV.
  
- Ejemplo en Python para leer un CSV
  
python
Copiar código
import csv

with open('archivo.csv', newline='', encoding='utf-8') as archivo:
    lector = csv.reader(archivo)
    for fila in lector:
        print(fila)

        
- Ejemplo en Python para escribir un CSV
  
python
Copiar código
import csv

datos = [
    ["Nombre", "Edad", "Ciudad"],
    ["Juan", 25, "Madrid"],
    ["Ana", 30, "Buenos Aires"]
]

with open('archivo.csv', 'w', newline='', encoding='utf-8') as archivo:
    escritor = csv.writer(archivo)
    escritor.writerows(datos)
    
## Ventajas del formato CSV
✔️ Ligero y fácil de manipular

✔️ Compatible con muchas aplicaciones

✔️ Fácil de generar y procesar en código

## Desventajas del formato CSV
❌ No soporta formatos complejos como colores o fuentes

❌ No maneja bien datos con comas dentro de los valores (requiere comillas)

❌ No permite relaciones avanzadas entre datos (como bases de datos relacionales)

Si necesitas algo más avanzado, formatos como JSON o Excel pueden ser una mejor opción. 🚀







