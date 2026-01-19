# Machine-learning-practica-1
Tarea machine learning practica 1

## Descripción del Proyecto

Este repositorio contiene la plantilla para la documentación del Test de Minería de Datos. El objetivo es proporcionar un formato estructurado para responder las 30 preguntas obligatorias y las preguntas opcionales del examen práctico.

## ⚠️ Aviso de Seguridad

**IMPORTANTE para usuarios de Windows**: Existe una vulnerabilidad de seguridad en nbconvert (todas las versiones <= 7.16.6). 

**Recomendación**: Use el método alternativo de exportación desde la interfaz de Jupyter (File → Download as → HTML) en lugar del comando de línea.

👉 **Lea el archivo [SECURITY_ADVISORY.md](SECURITY_ADVISORY.md) para más detalles y soluciones alternativas.**

## Estructura del Repositorio

- `Codigos_Test_Minería_NombreApellido.ipynb` - Plantilla de Jupyter Notebook para documentar las respuestas con código
- `Codigos_Test_Minería_NombreApellido.html` - Exportación HTML del notebook
- `.gitignore` - Archivo de exclusión para Git

## Instrucciones de Uso

### 1. Preparación del Entorno

Asegúrate de tener instalado Python 3.x y las siguientes librerías:

**Opción 1 - Instalar desde requirements.txt (recomendado):**
```bash
pip install -r requirements.txt
```

**Opción 2 - Instalación manual:**
```bash
pip install jupyter notebook nbconvert numpy pandas scikit-learn matplotlib seaborn
```

### 2. Completar el Notebook

1. Abre el notebook `Codigos_Test_Minería_NombreApellido.ipynb` con Jupyter:
   ```bash
   jupyter notebook Codigos_Test_Minería_NombreApellido.ipynb
   ```

2. Reemplaza `[Nombre Apellido]` en el encabezado con tu información personal

3. Para cada pregunta:
   - Copia el enunciado de la pregunta en la sección de markdown
   - Implementa el código correspondiente en la celda de código
   - Añade comentarios explicativos
   - Ejecuta la celda para verificar que funciona correctamente

4. **Importante**: 
   - Todas las respuestas deben estar respaldadas por código ejecutable
   - Las respuestas sin código no serán contabilizadas
   - Se requiere una única respuesta por pregunta

### 3. Exportar a HTML

⚠️ **Nota de Seguridad**: Si usas Windows, consulta [SECURITY_ADVISORY.md](SECURITY_ADVISORY.md) para métodos seguros de exportación.

Una vez completado el notebook, expórtalo a HTML usando uno de estos métodos:

**Opción 1 - Interfaz de Jupyter (RECOMENDADO para Windows):**
1. Abre el notebook en Jupyter
2. Ve a: File → Download as → HTML (.html)
3. Guarda el archivo descargado

**Opción 2 - Línea de comandos (Linux/macOS):**
```bash
jupyter nbconvert --to html Codigos_Test_Minería_NombreApellido.ipynb
```

**Nota**: Para usuarios de Windows, evite usar la opción de línea de comandos debido a una vulnerabilidad de seguridad en nbconvert.

### 4. Renombrar Archivos

Antes de entregar, renombra los archivos con tu nombre y apellido real:

```bash
# Ejemplo:
mv Codigos_Test_Minería_NombreApellido.ipynb Codigos_Test_Minería_JuanPerez.ipynb
mv Codigos_Test_Minería_NombreApellido.html Codigos_Test_Minería_JuanPerez.html
```

## Estructura del Notebook

El notebook está organizado en las siguientes secciones:

### Parte I: Preguntas Obligatorias (8 puntos)
- **Preguntas 1-10**: Conceptos Básicos y Preprocesamiento
- **Preguntas 11-20**: Algoritmos de Clasificación y Evaluación
- **Preguntas 21-30**: Clustering y Técnicas Avanzadas

### Parte II: Preguntas Opcionales (2 puntos)
- Casos Analíticos Específicos
- Requieren análisis más profundo y visualizaciones

## Librerías Incluidas

El notebook incluye las siguientes librerías pre-configuradas:

- **Análisis de Datos**: numpy, pandas
- **Visualización**: matplotlib, seaborn
- **Machine Learning**: scikit-learn (clasificación, clustering, métricas, preprocesamiento)
- **Algoritmos**: Decision Trees, Random Forest, Logistic Regression, SVM, Naive Bayes, K-Means, DBSCAN, PCA

## Criterios de Evaluación

- **8 puntos**: 30 preguntas obligatorias
- **2 puntos**: Preguntas opcionales con casos analíticos
- **Sin penalización**: No hay descuento por errores
- **Requisito**: El código debe ser ejecutable y documentado

## Recomendaciones

1. Lee cada pregunta cuidadosamente antes de implementar el código
2. Documenta tu código con comentarios claros
3. Verifica que todas las celdas se ejecuten sin errores
4. Incluye visualizaciones cuando sea apropiado
5. Asegúrate de que el HTML exportado sea legible y completo
6. Guarda tu trabajo frecuentemente

## Soporte

Para preguntas sobre el uso del notebook o problemas técnicos, consulta la documentación de:
- [Jupyter Notebook](https://jupyter-notebook.readthedocs.io/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [Pandas](https://pandas.pydata.org/docs/)

## Entrega

Entrega ambos archivos:
1. `Codigos_Test_Minería_[TuNombre][TuApellido].ipynb`
2. `Codigos_Test_Minería_[TuNombre][TuApellido].html`

Además del archivo Excel con las respuestas según las instrucciones del examen.
