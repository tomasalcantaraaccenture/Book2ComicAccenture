# Book2Comic: Transformando Libros en Cómics

![Book2Comic](resources/book2comic_logo.png)

## Introducción

Bienvenido a **Book2Comic**, una herramienta innovadora que transforma libros en tiras cómicas utilizando técnicas avanzadas de procesamiento de lenguaje natural (NLP), modelos de lenguaje grande (LLMs) y modelos generativos de imágenes. Con una interfaz sencilla de Streamlit, esta herramienta permite generar cómics tanto localmente como mediante APIs como Hugging Face, adaptándose a diferentes configuraciones de hardware.

## Guía de Instalación

Sigue estos pasos para configurar y ejecutar Book2Comic:

### Paso 1: Clonar el Repositorio

Descarga o clona el repositorio desde la fuente proporcionada.

### Paso 2: Crear el Entorno Conda

Asegúrate de tener Conda instalado en tu sistema. Luego, crea el entorno usando el archivo `environment.yml` proporcionado:

```bash
conda env create -f environment.yml
```

Activa el entorno:

```bash
conda activate JPA
```

### Paso 3: Instalar Requerimientos Adicionales

Una vez configurado el entorno, instala dependencias adicionales para SpaCy:

```bash
python -m spacy download en_core_web_sm
```

### Paso 4: Crear un token de huggingface (permisos: read)

https://huggingface.co

## Guía de Uso

### Ejecutar la Aplicación

Inicia la interfaz de Streamlit con el siguiente comando:

```bash
streamlit run app.py
```

Abre la URL proporcionada en tu navegador para acceder a la interfaz. Desde allí, sigue las instrucciones paso a paso para subir tu libro y generar cómics.



## Características Principales

1. **Análisis del Libro**: Extrae personajes, atributos y diálogos del texto del libro.
2. **Generación de Escenas**: Crea descripciones detalladas para escenas y diálogos.
3. **Creación de Imágenes**: Produce visuales usando Stable Diffusion.
4. **Adición de Globos de Diálogo** (opcional): Agrega globos de texto a las escenas utilizando una CNN.

## Ejemplo de Libros

Recomendamos comenzar con libros como las historias cortas de Sherlock Holmes, disponibles [aqui](https://sherlock-holm.es/ascii/), para probar la funcionalidad de la herramienta. Se recomienda usar solo el fichero para la JPA sherlock.txt (que adjunto junto con el proyecto) ya que los demás son muy largos y tarda demasiado.

