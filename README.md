# Pipeline de Machine Learning con CI/CD 🚀

Este lab tiene como objetivo automatizar el entrenamiento y evaluación de un modelo de Machine Learning usando GitHub Actions como herramienta de CI/CD. Se evalúa y ejecuta el modelo con cada push.

## Archivos

- **train.py**: Entrena un modelo de clasificación usando el dataset Iris
- **evaluate.py**: Evalúa el modelo entrenado y evalúa funcionalidad
- **testAccuracy.py**: Test automático que se asegura de que el modelo tenga al menos un 70% de precisión
- **requirements.txt**: Dependencias necesarias para correr el proyecto (`scikit-learn`, `numpy`, `pytest`, etc.)
- **.github/workflows/ml-pipeline.yml**: Configuración del pipeline en GitHub Actions, que se encarga de automatizar todo el flujo

## Reflexión CI/CD en proyectos de Machine Learning

Las herramientas de CI/CD como GitHub Actions son muy útiles en proyectos de Machine Learning. Permiten automatizar cosas que normalmente se hacen a mano: 
entrenar el modelo, probarlo, y asegurarse de que todo está funcionando bien cada vez que se cambia el código o los datos.

Con GitHub Actions, se logra que el modelo se entrene automáticamente y que, si algo no va bien (por ejemplo, si la precisión del modelo baja de cierto punto), 
podamos darnos cuenta antes de que llegue a producción. Esto ayuda a disminuir riesgos y optimizar el tiempo al momento de trabajar.

Además, CI/CD nos facilita el trabajo colaborativo. Los miembros de un equipo pueden hacer cambios y el pipeline va a determinar automáticamente los resultados 
de los cambios.
