# Proyecto-Integrador
### Tutorial: Cómo ejecutar el código correctamente

Este tutorial explica paso a paso el proceso para ejecutar correctamente el código proporcionado. Los pasos incluyen desde la configuración del entorno hasta la ejecución final de los programas. Cada código puede ejecutarse de manera independiente.

---

#### Paso 1: Configurar el ambiente de Python

1. **Instalar Python**:
   - Descarga e instala Python desde el sitio oficial: [python.org](https://www.python.org/).
   - Asegúrate de instalar una versión compatible con tu código (por ejemplo, Python 3.8 o superior).
   - Durante la instalación, selecciona la opción de agregar Python al PATH.
---

#### Paso 2: Obtener los datasets requeridos

1. **Reúne los datasets necesarios:**
   - Verifica los nombres y formatos de los archivos que tu código necesita (por ejemplo: `.csv`, `.xlsx`, etc.).
   - Asegúrate de que los archivos estén completos y en buen estado (sin celdas corruptas o datos faltantes críticos).

2. **Ubica los datasets en tu entorno local:**
   - Coloca los archivos en un directorio accesible para tu código.
   - Asegúrate de conocer la ruta exacta de los datasets (por ejemplo: `C:\Usuarios\MiUsuario\datasets\archivo.csv`).

---

#### Paso 3: Configurar la función para leer archivos

1. **Verifica la función de lectura:**
   - Asegúrate de que tu código incluya una función que permita cargar los archivos. Por ejemplo:
     ```python
     import pandas as pd

     def cargar_dataset(ruta_archivo):
         return pd.read_csv(ruta_archivo)  # Cambia 'read_csv' si usas otro formato
     ```

2. **Prueba la función de lectura:**
   - Antes de ejecutar todo el programa, prueba la función para asegurarte de que el archivo se carga correctamente:
     ```python
     ruta = "C:\\Usuarios\\MiUsuario\\datasets\\archivo.csv"
     dataset = cargar_dataset(ruta)
     print(dataset.head())
     ```

3. **Ajusta las rutas según sea necesario:**
   - Si estás trabajando con rutas relativas, coloca los archivos en el mismo directorio que tu código o utiliza rutas dinámicas con bibliotecas como `os`:
     ```python
     import os

     ruta = os.path.join(os.getcwd(), 'datasets', 'archivo.csv')
     dataset = cargar_dataset(ruta)
     ```

---

#### Paso 4: Ejecutar los programas

1. **Verifica el código:**
   - Revisa que el código principal esté preparado para ejecutarse de manera independiente y tengas instaladas las librerias necesarias:
   - Para los códigos de GRU y LSTM se debe tener instalado Keras Tuner. Puedes ingresar esta línea de código para hacerlo:
  
   !pip install -q -U keras-tuner

2. **Ejecuta cada código de manera independiente:**
   - Usa tu entorno para ejecutar tu programa


3. **Verifica los resultados:**
   - Revisa la salida y asegúrate de que no haya errores.

4. **Repite el proceso para los otros códigos:**
   - Ejecuta cada programa individualmente, asegurándote de ajustar las rutas y configuraciones según corresponda.
---

Con estos pasos y buenas prácticas, deberías poder ejecutar tus programas de manera eficiente y sin problemas.

