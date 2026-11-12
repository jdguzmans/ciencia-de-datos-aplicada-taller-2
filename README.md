# ciencia-de-datos-aplicada-taller-2

## Integrantes:
| Nombre | Código |
|---|---|
| Juan David Guzmán | 201224442 |
| Andrés Felipe Méndez | 200611694 |


## Objetivo

Predecir el abandono de clientes bancarios y estimar si una campaña de retención focalizada genera más valor que contactar a toda la base.

## Alcance
El análisis utiliza churn.csv para preparar los datos, comparar modelos, interpretar sus predicciones y estimar el valor de distintas estrategias de retención. La proyección considera 20.000 clientes, 15 % de abandono y 30 % de eficacia de retención, con costos y resultados expresados en COP.

## Conclusiones (Insights)
En el escenario base, la campaña focalizada con un umbral de 0,45, seleccionado en validación y evaluado en prueba, proyecta COP 101,38 millones de valor neto en el primer año, frente a COP 13,80 millones al contactar a todos. En el escenario conservador conviene no realizar la campaña; en el favorable, la campaña masiva obtiene mayor valor neto en prueba. Se recomienda validar costos y retención incremental mediante un piloto con grupo de control.

## Organización del repositorio
ciencia-de-datos-aplicada-taller-2/
├── .gitignore
├── README.md
├── churn.csv
├── enunciado.pdf
├── notebook.ipynb
└── requirements.txt

## Descripción de los componentes

- churn.csv: datos de clientes utilizados para el análisis de abandono.
- notebook.ipynb: preparación de datos, entrenamiento, evaluación cuantitativa y cualitativa, y estimación de valor de la campaña.
- enunciado.pdf: instrucciones y requerimientos del taller.
- requirements.txt: dependencias de Python del ejercicio.
- README.md: descripción e instrucciones del proyecto.
- .gitignore: archivos y carpetas que Git debe excluir.

## Instrucciones de ejecución
1. Abrir la carpeta del repositorio en Visual Studio Code o Jupyter.
2. Desde la raíz del repositorio, instalar las dependencias en el entorno de Python que se usará como kernel:
   python -m pip install -r requirements.txt
3. Abrir notebook.ipynb, seleccionar el kernel del entorno y ejecutar Run All. Mantener churn.csv en la raíz del repositorio.
 * El notebook sigue este orden:
 * Entendimiento y preparación de los datos.
 * Entrenamiento de los modelos.
 * Análisis cuantitativo de resultados.
 * Análisis cualitativo de resultados.
 * Generación de valor: estrategias de contacto, umbral económico, punto de equilibrio y sensibilidad.