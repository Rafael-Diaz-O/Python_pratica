<div align="center">

# 🐍 Python Prática

**Cuaderno de aprendizaje personal en Python** — desde lo básico (variables, listas, diccionarios) hasta el uso de IA (Gemini, Groq), manejo de archivos, Pandas y JSON.

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![Google Colab](https://img.shields.io/badge/Google-Colab-yellow?logo=googlecolab)](https://colab.research.google.com/github/Rafael-Diaz-O/Python_pratica/blob/main/Untitled3.ipynb)

</div>

---

## 📝 ¿Qué es este repositorio?

Este repositorio es mi **cuaderno de práctica de Python**, hecho en Google Colab (`Untitled3.ipynb`). No es un proyecto con una única funcionalidad, sino una bitácora de aprendizaje: contiene ejercicios, desafíos y ejemplos comentados sobre distintos temas del lenguaje, ordenados de forma progresiva.

**El propósito de este README es servir de índice.** La próxima vez que vuelva a este repo, la idea es poder mirar la tabla de abajo y decir *"ah, aquí está la explicación sobre listas"*, *"aquí quedó el ejemplo de JSON"*, etc., sin tener que scrollear todo el notebook para encontrarlo.

> 📌 El notebook tiene **~217 celdas**. Los números de celda de la tabla son aproximados (pueden variar levemente si se agregan celdas nuevas), pero sirven como referencia rápida de "más o menos por dónde buscar".

---

## 📑 Índice de temas (mapa del notebook)

| # | Tema | Celdas aprox. | Qué vas a encontrar ahí |
|---|---|---|---|
| 1 | **Introducción a Python** | 2 – 16 | `print()`, concatenación de strings, variables, tipos de datos, conversión `str → int`, reglas de nombres de variables, condicionales básicas (`if`/`else`) |
| 2 | **Uso de IA (Google Gemini)** | 18 – 29 | Conexión a la API de Gemini (`google.genai`), envío de prompts, creación de un chat (`client.chats.create`), historial de conversación, chatbot básico |
| 3 | **Listas** | 30 – 46 | Crear listas, acceder por índice (incluido índice negativo), `len()`, `append()`, `extend()` vs `append()` con listas, `remove()`, `pop()` (por posición y por defecto) |
| 4 | **Diccionarios** | 47 – 57 | Crear diccionarios, acceder por clave, `.items()`, `.keys()`, `.values()`, `.pop()`, diccionarios dentro de listas |
| 5 | **Ciclo `for`** | 58 – 60 | Recorrer listas y diccionarios con `for` |
| 6 | **Funciones** | 61 – 79 | `def`, parámetros, `return`, funciones que limpian texto (`.split()`, `.join()`), funciones combinadas con datos aleatorios (`random`) |
| 7 | **Desafío: resumidor de emails con IA** | 80 – 89 | Función que recibe una lista de emails y usa un LLM para resumirlos |
| 8 | **Modelos open source con Groq** | 90 – 98 | Instalación y uso de la librería `groq`, uso de `userdata` de Colab para manejar API keys de forma segura |
| 9 | **Manejo de archivos `.txt`** | 99 – 107 | Crear archivos, distintas formas de leerlos (`readlines()`, lectura completa, con/sin saltos de línea `\n`) |
| 10 | **Pandas – DataFrames** | 108 – 146 | `pd.read_csv()`, `.head()`, `.tail()`, selección de columnas, `.unique()`, `set()`, filtros con condiciones (`&`), `.shape` |
| 11 | **`iloc` y `loc`** | 148 – 167 | Diferencia entre indexar por posición (`iloc`) y por etiqueta (`loc`), slicing de filas, `set_index()`, selección de filas y columnas combinadas |
| 12 | **Desafío: clasificación de sentimiento con LLM + Pandas** | 172 – 193 | Cargar un CSV de reseñas, mandarlas a un LLM para clasificar sentimiento (positivo/negativo/neutro), guardar el resultado en el DataFrame |
| 13 | **Gestión de errores** | 194 – 207 | Bloques `try` / `except`, filtrar un DataFrame por condición, unir textos con un separador (`"###".join(...)`), categorización de texto |
| 14 | **JSON** | 208 – 214 | Qué es JSON y para qué sirve (conectar frontend/backend), `import json`, convertir texto con formato JSON en listas de diccionarios de Python |
| 15 | **Desafío Final (IDE local, no Colab)** | 215 en adelante | Leer un `.txt` línea por línea → lista de Python → mandar cada línea a un LLM local → recibir JSON con `usuario`, `reseña original`, `reseña_es` y `evaluación` |

---

## 🧭 Cómo usar este índice

1. Abre el notebook: [`Untitled3.ipynb`](https://github.com/Rafael-Diaz-O/Python_pratica/blob/main/Untitled3.ipynb) (o directo en [Google Colab](https://colab.research.google.com/github/Rafael-Diaz-O/Python_pratica/blob/main/Untitled3.ipynb)).
2. Usa `Ctrl/Cmd + F` y busca el título del tema (por ejemplo `Diccionarios:`, `Ciclo For`, `#JSON`, `#Gestion de errores`) — todos estos títulos están escritos como celdas de markdown dentro del notebook, así que aparecen tal cual en la tabla de contenidos de Colab/Jupyter (ícono ☰ a la izquierda).
3. Si buscas un **concepto de Python en general** (no un desafío), usa la tabla de arriba para saber en qué rango de celdas está.

---

## 🛠 Tecnologías y librerías usadas

| Librería / Herramienta | Para qué se usa en el notebook |
|---|---|
| **Python 3** | Lenguaje base |
| **Google Colab** | Entorno donde se escribió y ejecutó el notebook |
| **`google.genai`** | Conexión con los modelos Gemini de Google |
| **`groq`** | Conexión con modelos open source alojados en Groq (alternativa gratuita/rápida a Gemini) |
| **`pandas`** | Manipulación de datos tabulares (CSV, filtros, `iloc`/`loc`) |
| **`json`** | Conversión entre texto y estructuras de datos (listas/diccionarios) |
| **`random`** | Generación de datos aleatorios para ejercicios |
| **`os`** | Manejo de variables de entorno y archivos del sistema |

---

## 🚀 Cómo ejecutar el notebook

### Opción A — Google Colab (recomendado, es donde se creó)

1. Abre el notebook directamente en Colab con este [enlace](https://colab.research.google.com/github/Rafael-Diaz-O/Python_pratica/blob/main/Untitled3.ipynb).
2. Ve a **Entorno de ejecución → Ejecutar todo**, o ejecuta celda por celda con `Shift + Enter`.
3. Las celdas que usan IA (Gemini o Groq) necesitan una **API key** configurada como *secret* de Colab (ícono de llave 🔑 en el panel izquierdo) antes de poder ejecutarse.

### Opción B — Local (Jupyter / VS Code)

```bash
git clone https://github.com/Rafael-Diaz-O/Python_pratica.git
cd Python_pratica
pip install jupyter pandas google-genai groq
jupyter notebook Untitled3.ipynb
```

> ⚠️ Algunas celdas usan `google.colab.userdata`, que solo existe dentro de Colab. Si lo corres localmente, esas celdas necesitan adaptarse para leer la API key desde una variable de entorno (`os.environ`) en vez de `userdata.get(...)`.

---

## 🗺 Ideas para seguir practicando

- [ ] Separar cada tema en notebooks individuales (`01_listas.ipynb`, `02_diccionarios.ipynb`, etc.) para que sea más fácil de navegar.
- [ ] Agregar comprensión de listas (*list comprehensions*).
- [ ] Practicar clases y programación orientada a objetos (POO).
- [ ] Sumar manejo de expresiones regulares (`re`).
- [ ] Documentar los desafíos con su enunciado y solución en celdas de markdown separadas (actualmente algunos están mezclados con el código).

---

<div align="center">

Cuaderno de práctica de [Rafael-Diaz-O](https://github.com/Rafael-Diaz-O)

</div>
