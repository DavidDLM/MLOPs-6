# Pipeline de Machine Learning con CI/CD 🚀

Este lab tiene como objetivo automatizar el entrenamiento y evaluación de un modelo de Machine Learning usando GitHub Actions como herramienta de CI/CD. Se evalúa y ejecuta el modelo con cada push.

## Archivos

- **train.py**: Entrena un modelo de clasificación usando el dataset Iris
- **evaluate.py**: Evalúa el modelo entrenado y evalúa funcionalidad
- **testAccuracy.py**: Test automático que se asegura de que el modelo tenga al menos un 70% de precisión
- **requirements.txt**: Dependencias necesarias para correr el proyecto (`scikit-learn`, `numpy`, `pytest`, etc.)
- **.github/workflows/ml-pipeline.yml**: Configuración del pipeline en GitHub Actions, que se encarga de automatizar todo el flujo

## Reflexión CI/CD en proyectos de Machine Learning

Las herramientas de CI/CD como GitHub Actions son muy útiles en proyectos de Machine Learning. Permiten automatizar tareas que normalmente se hacen a mano, como entrenar el modelo, probarlo y asegurarse de que todo funciona bien cada vez que se cambia el código o los datos.

Con GitHub Actions, el modelo se entrena automáticamente, y si algo no sale bien (por ejemplo, si la precisión baja de cierto punto), nos damos cuenta antes de que llegue a producción. Esto ayuda a reducir riesgos y optimiza el tiempo al momento de trabajar.

Además, CI/CD facilita el trabajo colaborativo. Los miembros del equipo pueden hacer cambios y el pipeline determinará automáticamente los resultados de esos cambios, asegurando que todo siga funcionando correctamente.
