# DEEP LEARNING: libro de RNN, LSTM y aplicaciones

**Docente:** Keyla Vanessa Alba Molina  
**Departamento:** Matemáticas, Física y Ciencia de Datos  
**Institución:** Universidad del Norte

## Contenido

- `RNN_LSTM_Model_revisado.ipynb`: teoría de RNN y LSTM.
- `Aplicacion_NLP_Kalbam.ipynb`: aplicación a NLP, tareas y proyectos.
- `Aplicacion_Series_Tiempo_Original.ipynb`: aplicación LSTM a series de tiempo.
- `_static/`: logo, fotografía proporcionada por la docente y estilos visuales.
- `imgs/`: diagramas de los capítulos.
- `.github/workflows/publicar-libro.yml`: compilación y publicación en GitHub Pages.

## Fotografía y enlace institucional

Se incorporó la fotografía proporcionada por la docente en `_static/foto_docente.png`.
La fotografía y el nombre de la barra lateral, así como la fotografía de la portada,
redirigen al enlace solicitado de la Universidad del Norte. El destino corresponde
a la página de la Maestría en Estadística Aplicada.

## Compilar localmente

```bash
python -m pip install -r requirements.txt
jupyter-book build .
```

El libro compilado se guarda en `_build/html/`. La ejecución automática de
notebooks está desactivada para conservar el código y evitar entrenamientos durante
la compilación.

## Publicar con GitHub Actions

Descomprima el ZIP y suba **el contenido de esta carpeta**, incluida `.github`, a la
raíz del repositorio. En `Settings > Pages > Source`, seleccione `GitHub Actions`.
El flujo se ejecuta en la rama `main`; si su rama tiene otro nombre, cambie esa
línea en `.github/workflows/publicar-libro.yml`.

GitHub no ejecuta automáticamente un flujo que permanezca dentro de un ZIP sin
descomprimir. Si prefiere subir solo el ZIP, debe crear el flujo por separado y
hacer que lo descomprima.

## Alcance de las comprobaciones

No se modificaron las celdas de código ni el contenido de los tres notebooks.
Se comprobaron rutas de figuras, citas y etiquetas de forma estática; la
compilación completa no se ejecutó en este entorno porque no cuenta con Jupyter
Book y Sphinx. Dos referencias heredadas conservan la autoría pendiente de cotejo,
tal como se indica en `referencias.bib`. El flujo de NLP en portada es un esquema
recomendado; el código original mantiene las observaciones registradas en el capítulo.
