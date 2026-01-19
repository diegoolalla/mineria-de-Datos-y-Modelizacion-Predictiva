# Guía Rápida - Test de Minería de Datos

## 🚀 Inicio Rápido

### ⚠️ Aviso de Seguridad
**Usuarios de Windows**: Existe una vulnerabilidad en nbconvert. Use la interfaz de Jupyter para exportar HTML en lugar del comando de línea. Ver [SECURITY_ADVISORY.md](SECURITY_ADVISORY.md).

### 1. Instala las dependencias
```bash
pip install -r requirements.txt
```

### 2. Abre el notebook
```bash
jupyter notebook Codigos_Test_Minería_NombreApellido.ipynb
```

### 3. Completa las preguntas
- Copia el enunciado en la celda de markdown
- Escribe tu código en la celda de código
- Ejecuta la celda (Shift + Enter)
- Verifica que funciona correctamente

### 4. Exporta a HTML

⚠️ **IMPORTANTE - Usuarios de Windows**: Lee [SECURITY_ADVISORY.md](SECURITY_ADVISORY.md) primero.

**Método Seguro (Todos los sistemas):**
1. En Jupyter: File → Download as → HTML (.html)

**Método alternativo (Solo Linux/macOS):**
```bash
jupyter nbconvert --to html Codigos_Test_Minería_NombreApellido.ipynb
```

### 5. Renombra los archivos
Reemplaza "NombreApellido" con tu nombre real:
```bash
mv Codigos_Test_Minería_NombreApellido.ipynb Codigos_Test_Minería_TuNombre.ipynb
mv Codigos_Test_Minería_NombreApellido.html Codigos_Test_Minería_TuNombre.html
```

## 📝 Estructura del Test

### Parte I: Preguntas Obligatorias (8 puntos)
- **Preguntas 1-10**: Conceptos Básicos y Preprocesamiento
- **Preguntas 11-20**: Algoritmos de Clasificación y Evaluación
- **Preguntas 21-30**: Clustering y Técnicas Avanzadas

### Parte II: Preguntas Opcionales (2 puntos)
- Casos Analíticos Específicos
- Requieren análisis más profundo

## ✅ Lista de Verificación

Antes de entregar, asegúrate de:

- [ ] Has completado todas las 30 preguntas obligatorias
- [ ] Cada pregunta tiene código que se ejecuta sin errores
- [ ] Has añadido comentarios explicativos en el código
- [ ] Has actualizado tu nombre en el encabezado del notebook
- [ ] Has ejecutado todas las celdas en orden
- [ ] Has exportado el notebook a HTML
- [ ] Has renombrado ambos archivos con tu nombre real
- [ ] El archivo HTML se visualiza correctamente en un navegador

## 💡 Consejos

1. **Lee cada pregunta cuidadosamente** antes de escribir código
2. **Prueba tu código** en cada celda antes de continuar
3. **Comenta tu código** para explicar qué hace
4. **Usa visualizaciones** cuando sea apropiado (gráficos, tablas)
5. **Guarda tu trabajo frecuentemente** (Ctrl + S)
6. **No elimines** las celdas de instrucciones iniciales

## ⚠️ Importante

- **Las respuestas sin código no cuentan**: Todas las respuestas deben estar respaldadas por código ejecutable
- **Sin penalización por errores**: Intenta todas las preguntas
- **Una respuesta por pregunta**: Selecciona tu mejor solución

## 🔧 Problemas Comunes

### El notebook no se abre
```bash
# Reinstala Jupyter
pip install --upgrade jupyter notebook
```

### Error al importar librerías
```bash
# Reinstala las dependencias
pip install -r requirements.txt
```

### El HTML no se genera
```bash
# Instala nbconvert
pip install --upgrade nbconvert
```

## 📚 Recursos Útiles

- [Documentación de Jupyter](https://jupyter-notebook.readthedocs.io/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [Pandas](https://pandas.pydata.org/docs/)
- [Matplotlib](https://matplotlib.org/stable/contents.html)

## 🆘 ¿Necesitas Ayuda?

Si encuentras problemas:
1. Lee el archivo README.md para instrucciones detalladas
2. Revisa el ejemplo en la Pregunta 1 del notebook
3. Consulta la documentación de las librerías

---

**¡Éxito en tu test!** 🎓
