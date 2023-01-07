<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Eliel0328/2021-B065-Servidor-Web">
    <img src="./icon/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">
  Trabajo Terminal 2021-B065: Detector de texto ofensivo durante la navegación Web - API de clasificación</h3>

  <p align="center">
  <a href="https://github.com/Eliel0328/2021-B065-Servidor-Web"><strong>Revisar documento técnico »</strong></a>
  <br>
  <br>
  <a href="https://github.com/Eliel0328/2021-B065-Servidor-Web/issues">Reportar Error</a>
    ·
    <a href="https://github.com/Eliel0328/2021-B065-Servidor-Web/issues">Solicitar Función</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Contenido</summary>
  <ol>
    <li>
      <a href="#acerca-del-proyecto">Acerca del Proyecto</a>
      <ul>
        <li><a href="#api-de-clasificación">Api de clasificación</a></li>
      </ul>
      <ul>
        <li><a href="#desarrollado-con">Desarrollado Con</a></li>
      </ul>
    </li>
    <li>
      <a href="#guía-de-instalación">Guía de Instalación</a>
      <ul>
        <li><a href="#prerequisitos">Prerequisitos</a></li>
        <li><a href="#instalación">Instalación</a></li>
      </ul>
    </li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## Acerca del Proyecto


<p style="text-align: justify;">
La creciente relación humana con los medios digitales nos ha llevado a una dependencia de esta tal que su uso no se ha limitado por edades dado que en la actualidad es necesario en algunos casos que los niños hagan uso de estas herramientas, dejándolos expuestos a un posible encuentro con lenguaje ofensivo en modo texto o en su defecto manejar lenguaje ofensivo
</p>

<p style="text-align: justify;">
Para entender qué es el lenguaje ofensivo se debe revisar antes la definición de sus componentes, por lo tanto, según definiciones de la RAE el lenguaje es la facultad del ser humano de expresarse y comunicarse con los demás a través del sonido articulado o de otros sistemas de signos, es un sistema de comunicación que tiene como característica un estilo y modo de hablar y escribir de cada persona en particular. Mientras que la definición de un acto ofensivo sería todo aquel que tenga como objetivo humillar o herir el amor propio o la dignidad de alguien, puede considerarse también actos donde se dañen físicamente o maltraten a otra persona. Por lo tanto, en este trabajo el lenguaje ofensivo se definirá como “todas aquellas expresiones, palabras o texto que sean discriminatorias, despectivas y que tengan como propósito dañar a otra persona o grupo”.
</p>

<p style="text-align: justify;">
El sistema detecta el contenido de la navegación de los tutorados y notifica al tutor si se trata o hace uso de lenguaje ofensivo. Nuestro sistema se une a los diversos sistemas que tienen como objetivo detectar un acto ofensivo o discriminatorio los cuales se enfocan en detectar actos como el bullying, el acoso, el sexismo, racismo o algún otro acto ofensivo o denigrante. La diferencia sustancial es el método empleado para detectar su tema, en nuestro caso el lenguaje ofensivo es detectado por medio del análisis del texto de la página web, otra diferencia es el acto posterior al detectarlo pues lo que se realiza en nuestro sistema es enviar una notificación al tutor para que su criterio sea usado para juzgar el contenido visitado. De esta manera actos como el acosar o ser acosado en redes sociales, seguir discursos de odio, presenciar casos de racismo o participar en ellos, acceder a contenido para adultos, entre otras actividades podrían ser detectadas, prevenidas y discutidas por los involucrados (tutor y tutorado) para llegar a la mejor solución posible sin invadir la navegación o censurar el contenido directamente.
</p>

## API de clasificación

La API de clasificación trabaja en forma conjunta al resto del sistema. Las funciones realizadas son las siguientes:

- Recibe y limpia el texto a clasificar.
- Clasifica el texto en tres categorias [Ofensivo, Vulgar y Agresivo].
- Regresa en valor booleano el resultado de clasificación.

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>

### Desarrollado con

En esta sección se listan los principales frameworks utilizados para el arranque y desarrollo de la api de clasificación.


-   ![Python](https://img.shields.io/badge/python-6DA55F?style=for-the-badge&logo=python&logoColor=white)
-   ![Flask](https://img.shields.io/badge/flask-1c341a?style=for-the-badge&logo=flask&logoColor=white)
-   ![Scikit](https://img.shields.io/badge/scikit-575eaf?style=for-the-badge&logo=scikit&logoColor=white)
-   ![Pandas](https://img.shields.io/badge/pandas-080911?style=for-the-badge&logo=pandas&logoColor=white)

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>

<!-- GETTING STARTED -->

## Guía de instalación

Este es un ejemplo de configuracion. 


### Prerequisitos

-   `Python 3.0` o superior
-   `Git` 

### Instalación

_A continuación se muestran algunas opciones del proceso de instalación_


2. Clonar el repositorio.
   ```sh
   git clone https://github.com/Eliel0328/2021-B065-Clasificador.git
   ```
3. Usar pip y python para instalar los paquetes.
   ```
   pip install spacy pandas unidecode matplotlib sklearn flask
   python -m spacy download es_core_news_md
   ```
4. Correr el clasificador.
   
   ```
   python3 app.py
   ```



<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>