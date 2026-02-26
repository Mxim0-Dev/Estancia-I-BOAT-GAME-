# ESTANCIA I: BOAT-GAME (Originalmente llamado BOTE)

<p align="center">
  <img src="imagenes/TITULO.ico" alt="Logo" width="200">
</p>

<h3 align="center">Tecnologias usadas</h3>
<p align="center">
  <img src="https://img.shields.io/badge/Python_3.11-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pygame_2.5.2-ED1C24?style=for-the-badge&logo=pygame&logoColor=white" alt="Pygame">
  <img src="https://img.shields.io/badge/VISUAL_STUDIO-5C2D91?style=for-the-badge&logo=visual-studio&logoColor=white" alt="Visual Studio">
  <img src="https://img.shields.io/badge/PyInstaller-FFD43B?style=for-the-badge&logo=python&logoColor=3776AB" alt="PyInstaller">
</p>

<p align="center">
  <b>Lenguaje:</b> Python 3.11 &nbsp;&nbsp; | &nbsp;&nbsp; <b>Librería:</b> Pygame 2.5.2 &nbsp;&nbsp; | &nbsp;&nbsp; <b>IDE:</b> Visual Studio 2022 &nbsp;&nbsp; | &nbsp;&nbsp; <b>Empaquetado:</b> PyInstaller
</p>


Este proyecto fue desarrollado como parte de mi **Primera Estancia** académica para la carrera de **Ingeniería en Sistemas Computacionales** en la **Universidad Politecnica de Apodaca**. Consiste en una aplicación de escritorio diseñada en **Python** utilizando la librería **Pygame**, orientada a la concienciación sobre la limpieza de residuos en cuerpos de agua.


## Propósito
El propósito principal fue crear una herramienta interactiva que permitiera visualizar el impacto de la contaminación por plásticos en entornos acuáticos. El juego permite al usuario controlar un barco recolector para retirar botellas y bolsas de plástico, evitando colisiones con peces que representan la fauna afectada por la contaminacion.

<p align="center">
  <img src="imagenes/Captura.PNG" alt="GamePlay" width="1000">
  <br>
  <em>Captura del GamePlay.</em>
</p>

---



## Características Técnicas

Durante el desarrollo se implementaron soluciones técnicas específicas para garantizar un funcionamiento fluido en sistemas de escritorio:

* **Sistema de Probabilidad de Spawning**: Se implemento una lógica basada en el modulo `random` para enviar enemigos y plásticos de forma dinámica y aleatoria.
* **Gestión de Colisiones y Puntuación**: 
    * **Residuos Plásticos**: Cada recolección suma puntos y permite recuperar el margen de plasticos que se le pueden escapar al jugador.
    * **Colisión con Enemigos**: Reduce la salud del jugador, finalizando el juego si este llega a cero.
* **Manejo Dinámico de Recursos**: Se uso de un modulo de rutas para asegurar la carga de imágenes tanto en entorno de desarrollo como en el ejecutable final.
* **Sistema de Colisiones:** Se uso `spritecollide` para diferenciar entre recolectables (plásticos) y enemigos (peces).


## Creacion de los sprites: 
Uno de los mayores desafios fue la creacion de la identidad visual sin software de diseño especializado en pixel art:
* **Pipeline de Arte:** Los recursos vistos en la carpeta "imagenes" se crearon celda por celda en **Microsoft Excel** y se exportaron como archivos `.png` y despues convertidos a `.bmp`.
* **Gestión de Transparencia:** Debido a que en excel no se pueden hacer celdas transparentes para el fondo, se opto por hacer a los bordes de los sprites del color exacto del fondo donde se posicionaran, esto para mimetizarse con la imagen del fondo. Pero al mismo tiempo generando unos bugs visuales curiosos.

<p align="center">
  <img src="imagenes/CapturaMapa.png" alt="Mapa" width="900">
  <br>
  <em>Diseño del mapa en Excel.</em>
</p>
<p align="center">
  <img src="imagenes/CapturaSprites.png" alt="Sprites" width="900">
  <br>
  <em>Diseño de sprites en Excel.</em>
</p>



## Cómo ejecutar
Descarga la versión estable desde la sección de [Releases](https://github.com/Mxim0-prog/Estancia-I-BOAT-GAME-/releases) y ejecuta `Bote.exe`.

## Arquitectura del Proyecto

La organización del repositorio sigue un estándar modular para facilitar el mantenimiento y la exportación de recursos:

```text
├── 📂imagenes/          # Recursos visuales
├── 📄ajustes.py         # Configuración de velocidades, probabilidades y dimensiones
├── 📄barco.py           # Lógica y control del jugador
├── 📄Bote.py            # Script principal y bucle del juego
├── 📄enemigo.py         # Definición de la entidad enemiga
├── 📄plasticos.py       # Definición de las entidades recolectables 
├── 📄resources.py       # Permite encintrar la ruta de los recursos visuales
└── 📄README.md          # Documentación técnica
```

## Evolución hacia B0AT-MOBILE (Estancia II)
Este repositorio es el testimonio de mi crecimiento tecnico. Las lecciones aprendidas aqui sobre hitboxes, logica de estados, diseño de HUD, etc. Fueron un pilar fundamental para el desarrollo **B0AT** en mi Estancia II, donde migre a **Godot Engine** para una experiencia más robusta, su exportacion a dispositivos mobiles.


---
<p align="center">
  <b>¿Te gustó mi trabajo? ¡Conectemos!</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/maximo-juarez-rodríguez-8911b3327">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="https://github.com/Mxim0-Dev">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="mailto:mxoju07@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>
</p>


<p align="center">
  Desarrollado por <b>Maximo Juarez Rodriguez</b> – Estudiante de Ingeniería en Sistemas Computacionales, UPAPNL 2024.
</p>
