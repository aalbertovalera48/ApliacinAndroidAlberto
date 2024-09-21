# README - Alberto Valera- Aplicación Android Básica
## Link al Repositorio GitHub: 
## Ejercicio Individual

### Objetivo General
Desarrollar competencias en la creación de aplicaciones Android utilizando Programación Dirigida por Eventos, enfocándose en la experiencia del usuario y la interacción con la interfaz.

### Objetivos Específicos
- Comprender el entorno de desarrollo Android Studio y sus componentes.
- Diseñar y desarrollar interfaces de usuario interactivas.
- Implementar el manejo de eventos en aplicaciones Android.
- Realizar pruebas y depuración de aplicaciones Android.

## Enunciado

### Tema 1: Primeros Pasos y Experiencia de Usuario

Esta actividad se centra en la creación de una aplicación básica en Android que permite a los estudiantes aplicar los conocimientos adquiridos en esta unidad.

### Funcionalidades Básicas de la Aplicación
1. **Pantalla de Inicio:**
   - Un saludo personalizado que cambia según la hora del día (Buenos días, Buenas tardes, Buenas noches).
   - Un botón que lleva a la pantalla de la actividad principal.

2. **Actividad Principal:**
   - Un campo de texto para ingresar el nombre del usuario.
   - Un botón para guardar el nombre ingresado.
   - Un TextView que muestra el nombre ingresado.
   - Un botón para navegar a una tercera pantalla.

3. **Pantalla de Configuración:**
   - Opciones para cambiar el color del fondo de la aplicación.
   - Un botón para volver a la pantalla de inicio.

## Estructura del Código

### 1. `MainActivity.kt`
La actividad principal de la aplicación, donde el usuario puede ingresar su nombre. Incluye un campo de texto para la entrada del nombre, un botón para guardarlo y un botón que permite navegar a la pantalla de configuración.

### Descripción:

**MainActivity:** La clase principal que contiene la lógica para gestionar el estado del nombre ingresado por el usuario.

**MainScreen:** Una función composable que presenta la interfaz de usuario. Permite la entrada de texto y la navegación a otras pantallas.

### 2. `SplashScreenActivity.kt`
Esta clase muestra una pantalla de bienvenida que saluda al usuario según la hora del día. Proporciona un botón para navegar a la MainActivity.

### Descripción:

**SplashScreenActivity:** Muestra un saludo personalizado al usuario, dependiendo de la hora del día.

**SplashScreen:** Función composable que presenta el saludo y un botón para continuar hacia la actividad principal.

### 3. `PantallaConfiguraciónActivity.kt`
Esta actividad permite a los usuarios cambiar el color de fondo de la aplicación y regresar a la pantalla de inicio(SplashScreenActivity).

### Descripción:

**PantallaConfiguracionActivity:** Esta clase gestiona la pantalla de configuración, permitiendo al usuario cambiar el color de fondo de la aplicación.

**SettingsScreenContent:** Función composable que encapsula el contenido de la pantalla de configuración.

### 4. `PantallaConfiguración.kt`
En esta clase, el usuario puede seleccionar un color de fondo y regresar a la pantalla principal. Se manejan los cambios de estado para el color seleccionado.

#### Descripción:

**PantallaConfiguracion:** Esta función permite al usuario seleccionar el color de fondo y regresar a la pantalla principal.

**SeleccionColor:** Muestra opciones de colores y gestiona la selección del usuario, cambiando el estado del color de fondo.

### 5. `Almacenamiento y Configuración`
Las funciones saveBackgroundColor y getBackgroundColor permiten almacenar y recuperar el color de fondo seleccionado utilizando SharedPreferences.

#### Descripción:

**saveBackgroundColor:** Esta función guarda el color de fondo seleccionado en las preferencias compartidas, lo que permite recordar la elección del usuario entre sesiones.

**getBackgroundColor:** Recupera el color de fondo almacenado, aplicando el color correcto al iniciar la aplicación.


## Conclusión:
La creación de esta aplicación Android básica ha permitido consolidar una serie de competencias fundamentales en el desarrollo de software móvil, centrándose especialmente en la Programación Dirigida por Eventos y en la mejora de la experiencia del usuario. A través de un enfoque práctico, se ha logrado implementar características esenciales que no solo enriquecen la funcionalidad de la aplicación, sino que también fomentan la interacción y el compromiso del usuario.

## Aprendizajes Clave
- **Interacción con el Usuario:** La implementación de una interfaz amigable y accesible demuestra la importancia de diseñar aplicaciones que respondan adecuadamente a las necesidades y expectativas del usuario. Al ofrecer opciones personalizables, como la selección de color de fondo, se fomenta una mayor conexión con la aplicación.

- **Manejo de Estados y Navegación:** El uso de State y LiveData en Jetpack Compose ha facilitado la gestión del estado en tiempo real, permitiendo que la interfaz se actualice automáticamente en respuesta a las acciones del usuario. Esto refuerza la idea de que una buena arquitectura de aplicación debe centrarse en el flujo de datos y en cómo se reflejan en la interfaz.

- **Persistencia de Datos:** A través de SharedPreferences, se ha aprendido a almacenar información de manera eficiente, permitiendo que la configuración de la aplicación se mantenga entre sesiones. Esto no solo mejora la experiencia del usuario, sino que también sienta las bases para el manejo de datos más complejos en aplicaciones futuras.

- **Desarrollo Colaborativo y Mejora Continua:** Este ejercicio también ha resaltado la importancia del trabajo en equipo y la revisión de código. Al compartir y discutir soluciones, se promueve un entorno de aprendizaje dinámico que fomenta la innovación y la mejora continua en las habilidades de programación.

## Implicaciones Futuras
El desarrollo de esta aplicación no solo representa un ejercicio académico, sino que también abre la puerta a futuras exploraciones en el desarrollo de aplicaciones móviles. Las competencias adquiridas servirán de base para abordar proyectos más complejos, incluyendo la integración de APIs, bases de datos locales, y patrones de diseño avanzados. Asimismo, la experiencia adquirida en la implementación de interfaces reactivas y en la gestión del estado será invaluable al abordar desarrollos más ambiciosos.

## Reflexión Final
En un entorno tecnológico en constante evolución, es esencial mantenerse actualizado con las mejores prácticas y tendencias en el desarrollo de aplicaciones. Este ejercicio ha proporcionado una valiosa oportunidad para aplicar teoría en un contexto práctico, cimentando así un enfoque de aprendizaje que será crucial en el futuro profesional. La combinación de teoría y práctica, junto con una mentalidad de mejora continua, es lo que permite a los desarrolladores no solo adaptarse a los cambios, sino también liderar innovaciones en el campo del desarrollo de software.
