# Clasificacion-de-personajes-de-Los-Simpsons

Este repositorio contiene el desarrollo de una práctica académica realizada como parte de la asignatura **Minería de Datos** durante el curso 2023–2024, en el Grado en Ingeniería Informática.

### Autores:

* Alejandro Sánchez Corredor
* Iván Fernández García
  
---

### Descripción del Proyecto

El objetivo de esta práctica es aplicar técnicas de aprendizaje profundo para construir un modelo capaz de **clasificar imágenes de personajes de la serie *Los Simpsons***. Se emplea para ello la biblioteca `TensorFlow`, una de las más populares en el ámbito de las redes neuronales.

---

### Contenido de la libreta

* Comprobación del uso de GPU y fijación de semillas para reproducibilidad
* Preprocesamiento de imágenes
* Construcción de modelos **CNN** y **Transfer Learning**
* Aplicación de técnicas de aumento de datos
* Uso de callbacks y fine-tuning
* Evaluación con métricas y visualización de resultados
* Comparación de estrategias y mejora iterativa

---

### Tecnologías y Librerías Utilizadas

* Python
* TensorFlow
* NumPy
* Matplotlib
* Pandas
* scikit-learn

---

### Archivos

* `Clasificación de personajes de Los Simpsons.ipynb` – Libreta Jupyter con todo el desarrollo, modelos, entrenamientos y análisis final

---

### Resultados

El modelo final alcanzó una precisión superior al **90%**, gracias a la combinación de técnicas de aumento de datos, optimización con callbacks y el uso de modelos preentrenados mediante **Transfer Learning**.

---

### Conclusiones y Lecciones Aprendidas

Esta práctica ha sido nuestra **primera experiencia real con redes neuronales y TensorFlow**, y nos ha dejado grandes aprendizajes aplicables a proyectos futuros:

* **Importancia de la estratificación**: Garantizar que todas las clases estén bien representadas en entrenamiento y validación mejora significativamente la robustez del modelo. Para ello usamos `split-folders`.

* **Carga de datos en TensorFlow**: Exploramos distintas formas de preparar los datos, decantándonos por generadores desde directorio con aumento solo en entrenamiento, pero comprendiendo también otras estrategias como `image_dataset_from_directory`.

* **Aumento de datos (data augmentation)**: Demostró ser esencial para evitar sobreajuste y mejorar la generalización del modelo.

* **Uso de callbacks**: Nos permitió detener el entrenamiento de forma inteligente y conservar el mejor modelo validado.

* **Transfer Learning + Fine-Tuning**: El uso de modelos como InceptionV3 ha sido clave. Aunque al principio los resultados eran modestos, con fine-tuning y menor learning rate conseguimos nuestros mejores resultados.

* **CNN desde cero**: Aunque más costoso, construir nuestras propias redes nos permitió entender a fondo la arquitectura de una CNN y comparar su rendimiento frente a modelos preentrenados.

* **Iteración y experimentación**: El progreso vino de probar, ajustar y volver a intentar. No hubo una única solución perfecta, sino muchas pequeñas mejoras acumuladas.

* **Competencia como motivación**: Buscar el mejor modelo nos impulsó a aprender más, consultar notebooks de Kaggle, repositorios externos y documentación avanzada.

---

### Cómo ejecutar el proyecto

```bash
git clone https://github.com/tu-usuario/los-simpsons-clasificacion.git
cd los-simpsons-clasificacion

pip install -r requirements.txt
jupyter notebook
```
