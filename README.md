# Introducción a la Informática para Científicos — VIU

Materiales de la asignatura **Introducción a la Informática para Científicos** de la **Universidad Internacional de Valencia (VIU)**. El repositorio reúne notebooks con explicaciones, ejemplos de código y ejercicios para aprender los fundamentos de la informática y comenzar a programar en Python con aplicaciones científicas.

El recorrido parte del funcionamiento de los ordenadores y la formulación de algoritmos, y avanza hacia el cálculo numérico, la visualización de datos y las simulaciones. Está orientado a estudiantes que se inician en la programación.

## Objetivos de aprendizaje

- Comprender la representación de la información y los componentes básicos de un ordenador.
- Expresar algoritmos mediante pseudocódigo y diagramas de flujo, y comprobarlos con pruebas de escritorio.
- Utilizar variables, operadores y estructuras de datos de Python.
- Resolver problemas con condicionales, bucles, funciones y manejo de archivos.
- Trabajar con arrays de NumPy y representar resultados con Matplotlib.
- Introducir la organización del código en módulos, el manejo de excepciones y las clases.
- Documentar cálculos y resultados en notebooks mediante Markdown, LaTeX y HTML.

## Notebooks por temas

Todos los materiales se encuentran en [`notebooks/`](notebooks/), organizados por sus temas. El orden de la tabla propone un recorrido desde los fundamentos hasta el cálculo científico y las simulaciones. Algunos notebooks comparten contenidos y ofrecen ejemplos complementarios o un tratamiento más detallado.

| Notebook | Contenido | Ejecutar |
| --- | --- | --- |
| [Introducción a los ordenadores](notebooks/fundamentos_ordenadores.ipynb) | Historia de las computadoras, bits y bytes, lógica booleana y compuertas lógicas, arquitectura de von Neumann, sistemas operativos, hardware y modelos de computación. | [Abrir en Colab](https://colab.research.google.com/github/ssanchezgoe/intro_informatica_viu/blob/main/notebooks/fundamentos_ordenadores.ipynb) |
| [Introducción a Google Colab](notebooks/introduccion_google_colab.ipynb) | Celdas de código y texto; ejemplos de Python y comandos de shell; documentación con Markdown, LaTeX y HTML. | [Abrir en Colab](https://colab.research.google.com/github/ssanchezgoe/intro_informatica_viu/blob/main/notebooks/introduccion_google_colab.ipynb) |
| [Práctica de Colab y documentación científica](notebooks/practica_colab_documentacion_cientifica.ipynb) | Práctica complementaria de celdas y formato de texto, expresiones matemáticas y HTML. Incluye la densidad de una distribución gaussiana y su representación con Python. | [Abrir en Colab](https://colab.research.google.com/github/ssanchezgoe/intro_informatica_viu/blob/main/notebooks/practica_colab_documentacion_cientifica.ipynb) |
| [Algoritmos, variables, operadores y estructuras de datos](notebooks/algoritmos_variables_operadores_estructuras_datos.ipynb) | Algoritmia, pseudocódigo, diagramas de flujo y pruebas de escritorio. Variables, tipos de datos, operadores, cadenas, listas, diccionarios y tuplas, con ejemplos y ejercicios. | [Abrir en Colab](https://colab.research.google.com/github/ssanchezgoe/intro_informatica_viu/blob/main/notebooks/algoritmos_variables_operadores_estructuras_datos.ipynb) |
| [Condicionales, bucles, funciones y archivos](notebooks/condicionales_bucles_funciones_archivos.ipynb) | `if`, `elif`, `else`, `for`, `while`, control de bucles y comprensiones. Lectura y escritura de archivos, funciones, `*args`, `**kwargs`, expresiones lambda y ejercicios de recursión, Fibonacci y estimación de π por Monte Carlo. Incluye un ejemplo con pandas. | [Abrir en Colab](https://colab.research.google.com/github/ssanchezgoe/intro_informatica_viu/blob/main/notebooks/condicionales_bucles_funciones_archivos.ipynb) |
| [Módulos, excepciones, clases y cálculo científico](notebooks/modulos_excepciones_clases_calculo_cientifico.ipynb) | Módulos `math` y `random`, arrays y operaciones matriciales, gráficos y módulos propios. Manejo de excepciones y archivos con `with`; clases, atributos, métodos y constructores. Ejercicios de Monte Carlo y figuras geométricas. | [Abrir en Colab](https://colab.research.google.com/github/ssanchezgoe/intro_informatica_viu/blob/main/notebooks/modulos_excepciones_clases_calculo_cientifico.ipynb) |
| [NumPy, Matplotlib, clases y caminatas aleatorias](notebooks/numpy_matplotlib_clases_caminatas_aleatorias.ipynb) | Desarrollo más detallado de arrays: tipos, memoria, indexado, segmentación, cambio de forma, concatenación, vectorización y broadcasting. Gráficos de líneas, variables categóricas y dispersión, talleres, clases y simulación de una caminata aleatoria. | [Abrir en Colab](https://colab.research.google.com/github/ssanchezgoe/intro_informatica_viu/blob/main/notebooks/numpy_matplotlib_clases_caminatas_aleatorias.ipynb) |

## Aplicaciones científicas

Los ejemplos de **Monte Carlo** y **caminatas aleatorias** se utilizan en las sesiones 11–13 de aplicaciones a problemas físicos:

- **Monte Carlo:** estimación de π mediante muestreo aleatorio, en los notebooks de condicionales, bucles y funciones y de módulos, excepciones y clases.
- **Caminatas aleatorias:** simulación y representación de resultados, en el notebook de NumPy, Matplotlib y clases.

## Cómo trabajar con los materiales

### En Google Colab

1. Abre el enlace **Abrir en Colab** del notebook que quieras estudiar.
2. Guarda una copia en tu Google Drive para conservar tus cambios y las soluciones de los ejercicios.
3. Lee las explicaciones y ejecuta las celdas de código progresivamente con `Shift + Enter`.
4. Modifica los ejemplos y resuelve los ejercicios para comprobar lo aprendido.

Algunos ejercicios incluyen soluciones en comentarios de las celdas de texto, que se pueden consultar al editar la celda. Los ejemplos de archivos que usan `sample_data` o `google.colab` están pensados para el entorno de Colab. Descarga los archivos que quieras conservar antes de finalizar la sesión.

### En un entorno local con Jupyter

Para trabajar en tu ordenador, utiliza Python 3 y un entorno virtual. Desde la carpeta del repositorio, en macOS o Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install jupyterlab numpy matplotlib scipy pandas
jupyter lab
```

En Windows, activa el entorno con `.venv\Scripts\activate` en lugar de `source .venv/bin/activate`.

Abre el notebook deseado desde la carpeta `notebooks/`. NumPy y Matplotlib se utilizan para el cálculo y los gráficos; SciPy aparece en ejemplos de distribuciones y pandas en un ejemplo de transformación de datos. Los módulos de la biblioteca estándar, como `math`, `random`, `os` y `shutil`, no necesitan instalación adicional.

Para ejecutar localmente ejemplos específicos de Colab, adapta las rutas de archivos y sustituye las operaciones de subida y descarga por archivos de tu ordenador. Algunos ejemplos plantean errores o código incompleto como parte del aprendizaje; conviene ejecutarlos y analizarlos por separado.
