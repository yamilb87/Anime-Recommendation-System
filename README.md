![GitHub repo size](https://img.shields.io/badge/repo_size-135_mb-blue?logo=files&logoColor=yellow) 
![GitHub repo file count](https://img.shields.io/badge/files-7_files-blue?logo=files&logoColor=yellow)

---

# Sistema de Recomendación de Anime

![banner](Images/cover.png)

---

**Lenguajes**

[![GitHub laguage](https://img.shields.io/badge/jupyter_notebook-3C4048?logo=jupyter)](https://jupyter.org/)
[![GitHub laguage](https://img.shields.io/badge/python-3C4048?logo=python&logoColor=#3776AB)](https://www.python.org/)

---

**Librerías** 
>_principales_

[![GitHub laguage](https://img.shields.io/badge/numpy-gray?logo=numpy&labelColor=013243&style=for-the-badge)](https://numpy.org/)
[![GitHub laguage](https://img.shields.io/badge/pandas-gray?logo=pandas&labelColor=3776AB&style=for-the-badge&logoColor=white)](https://pandas.pydata.org/docs/)
[![GitHub laguage](https://img.shields.io/badge/scikit--learn-gray?logo=scikit-learn&labelColor=F7931E&style=for-the-badge&logoColor=white)](https://scikit-learn.org/)
[![GitHub laguage](https://img.shields.io/badge/scipy-gray?logo=scipy&style=for-the-badge&labelColor=8CAAE6&logoColor=white)](https://scipy.org/)


---

1. _**Abstracto**_:

   El siguiente estudio tiene como objetivo presentar un **[dataset de animes](Datasets)**, para ser utilizado en un sistema de recomendación. El dataset contiene información sobre _diferentes títulos de anime, incluyendo géneros, año de lanzamiento, calificaciones y reseñas de los usuarios_.

   Este dataset fue recolectado a través de varias fuentes en línea, incluyendo sitios web de anime y plataformas de calificación de usuarios. También se han incluido detalles sobre los creadores y productora de cada título.

   La información del dataset está compuesta por datos sobre las preferencias de unos 73000 usuarios entre unos 12300 animes aproximadamente.

   El sistema de recomendación se basará en la información contenida en el dataset, utilizando técnicas de aprendizaje automático para analizar los datos y generar recomendaciones personalizadas para los usuarios.

   En general, este dataset y el sistema de recomendación basado en él, ofrecerá a los usuarios la posibilidad de descubrir nuevos animes que puedan interesarles, basándose en su historial de visualización y preferencias personales. Además, también podría ser utilizado por los investigadores en el campo del aprendizaje automático y la recomendación para llevar a cabo sus propias investigaciones y mejorar el rendimiento del sistema.

---

2. _**Contenido - archivos principales**_
   
   * _[Datasets](Datasets)_
      * _[anime.csv](Datasets/anime.csv)_
      * _[rating.csv](Datasets/rating.csv)_         

   * _[Docs](Docs)_
      * _[Presentación ("Brief")](Docs/Brief.pptx)_

         * Contexto y Motivación del proyecto.
         * Hipótesis y preguntas de interés.
         * Breve Exploración de Datos.
         * Modelos de Motor de búsqueda aplicados.
         * Insights y Recomendaciones.
     
       * [_Relevo fitro_user_id.xlsx_](Docs/Relevo%20fitro_user_id.xlsx)
 
   * _[Images](Images)_

   * _[Jupyter Notebook](Anime_SystemRecommendation.ipynb)_
  
  --- 

3. _**Datasets**_

   * **[anime_data](Datasets/anime.csv)**

   | Nombre   | Descripción                                                                |
   |----------|----------------------------------------------------------------------------|
   | anime_id | id del anime (unívoco-PK)                                                  |
   | name     | nombre del anime                                                           |
   | genre    | lista de géneros (separados por coma) del anime                            |
   | type     | movie, OVA, TV, etc                                                        |
   | episodes | cantidad de episodios del anime (1 si es película)                         |
   | rating   | rating promedio (máx 10) del anime                                         |
   | members  | número de miembros de la comunidad que se encuentran en el grupo del anime |
   ---


   * **[rating_data]((Datasets/rating.csv))**

   | Nombre   | Descripción                                                                                             |
   |----------|---------------------------------------------------------------------------------------------------------|
   | user_id  | id del usuario (unívoco-PK)                                                                             |
   | anime_id | anime que el usuario ha puntuado                                                                        |
   | rating   | rating/puntuación otorgada por el usuario (-1 si el usuario no ha puntuado el anime - máx. valor de 10) |
   ---

---

4. _**Requisitos**_

   Para instalar las librerías necesarias, ejecutar el siguiente comando:
   ```
   pip install -r requirements.txt
   ```

---

5. _**Instrucciones de uso**_

   *  Descargar o clonar repositorio.
   ```
   git clone https://github.com/yamilb87/Anime-Recommendation-System.git
   ```
   * Instalar las dependencias utilizando el comando mencionado anteriormente.

   * Abrir el Jupyter Notebook _**`Anime_SystemRecommendation.ipynb`**_ en tu entorno de Jupyter.

   * Siguir las instrucciones dentro del notebook para ejecutar el sistema de recomendación de anime.

---

6. _**Trabajo futuro**_
   
   * Optimizar funciones y widgets del noteook.
  
   * Mejorar modelo de Filtrado colaborativo, incorporar datos del usuario para generar recomendaciones. Es decir que _cada usuario_, debería obtener _recomendaciones personalizadas_.
   
   * Realizar _app interactiva_, incorporando los modelos de recomendación (ej. _[Streamlit](https://streamlit.io/)_). 
   
---

7. _**Reconocimientos**_

   * A [_`myanimelist.net`_](https://myanimelist.net/) por la plataforma desarrollada que permitió la creación de los datasets utilizados. 

   * Al staff de _`Coderhouse`_ por el soporte en el desarrollo del curso y en el avance del proyecto.

---

8. _Dale una ⭐️ si te ha sido útil!_ 😉