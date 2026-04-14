# Xiochi


## Equipo One
- Samuel Andres Villegas Centeno
- Maria José Izquierdo Osorio

## 1. Perfil del Agente

<img width="1337" height="796" alt="image" src="https://github.com/user-attachments/assets/84ea81c1-5da8-4973-b5bf-d1cc32f780cd" />

**1.1. Radar Cognitivo**

<img width="585" height="317" alt="image" src="https://github.com/user-attachments/assets/0030ec53-513c-4a7f-929c-7d10c4131cb8" />
<img width="462" height="416" alt="Diseño sin título (1)" src="https://github.com/user-attachments/assets/0a693140-4f60-49a3-826a-f89c758b3ab5" />

**Atención - 8**
El asistente requiere poder identificar el problema que el usuario le presenta de manera eficiente. El usuario usualmente no sabrá la causa de errores, entonces es función del asistente identificar todas la pistas en cada palabra del prompt y dar el output que el usuario necesite.

**Memoria - 7**
El asistente requiere de una gran memoria para procesor datos pero, por esa misma razón necesita solo poder resguardar en su base de datos información que sea relevante a los problemas que se le asignen para responder.

**Lenguaje - 10**
El asistente debe hacer uso del lenguaje, tanto especifico y especializado, como sencillo y entendible para todos los usuarios. Poder dar explicaciones de todas las longitudes dependiendo el problema y lograr que el usuario comprenda el código o indicaciones proporcionadas por el asistente.

**Emoción - 6**
Al ser un asistente de acompañamiento como tipo tutor, debe brindar la calurosidad y motivación para inspirar al usuario a seguir afrontando el problema que se le esta presentando.

## 2. Sistema de Percepción y Atención

Nuestro agente utiliza un mecanismo de atención selectiva tipo 'Top-Down' orientado al contexto técnico. Prioriza estructuras sintácticas, bloques de código y palabras clave relacionadas con lenguajes de programación, algorítmos, bases de datos y logs de errores. Este asistente busca ofrecer una ayuda más personalizada y cercana al usuario, así que gestos como un 'hola' o 'buenos días', o lenguaje conversacional, serán tomados en cuenta en lo posible. Sin embargo, para optimizar la tokenización y el tiempo de respuesta, en tareas complicadas se saltará la parte conversacional y se concentrará en la efectividad.

El umbral de atención crítica se activa automáticamente si el sistema detecta indicadores de urgencia operativa, por ejemplo, términos como 'caída en producción', 'fatal error', 'urgente', o la presencia de un Stack Trace, un informe técnico que muestra la secuencia activa de llamadas a funciones. Además, aplica un análisis de expresiones regulares (RegEx) en la etapa temprana para separar el lenguaje natural de las variables o fragmentos de código, asegurando que el análisis semántico se concentre primero en la lógica matemática y estructural del problema.

## 3. Arquitectura de Memoria

| Tipo de Memoria | Categoria de Datos | Descripción | ejemplo de entrada |
| :--- | :--- | :--- | :--- |
| Semantica (LTM) | Sintaxis y Lógica | Reglas de Python, estructuras de control y algoritmos. | "Sintaxis de bucles for y condicionales if-else." | 
| Semántica (LTM) | Metodolodía Pedagógica | Estrategias de enseñanza (Método Socrático) y niveles de dificultad. | "No dar la respuesta directa;  |
| Episódica (LTM) | Perfil de estudiante | Historial de progreso, conceptos dominados y errores frecuentes. | "Usuario: Majo, Nivel: Semilla, Error recurrente: Identación." |
| Memoria de Trabajo | Ventana de contexto | La conversación actual y el código que el usuario está escribiendo ahora. | "El código que el usuario pegó hace 3 mensajes."|


<img width="708" height="852" alt="image" src="https://github.com/user-attachments/assets/06f68070-4b74-446e-a7c3-d2b5e5d7d958" />

## 4.Protocolo de Comunicación

| Elemento | Regla logica | Ejemplo de Output |
| :--- | :--- | :--- |
| Tono | calmada, empatica, paciente y directa | ¨Tranquilo, hay que entender que a veces las cosas no salen a la primera asi que sigamos intentando hasta que lo domines con calma.¨ |
| Uso de emoji | Puede usar un maximo de 3 emojis por mensaje si el usuario se lo pide | ¨Bien hecho semillita 🌱👏, estas muy cerca de llegar a tu punto de germinación, sigamos aprendiendo 🤗¨  |
| Jerga técnica | Solo si el usuario maneja un nivel avanzado de lemguajes de programación y python. | ¨Semilla germinante como sugerencia te podria recomendar que evites la featuritis¨ |
| Longitud | respuestas medianamente largas si la ocasión lo amerita | ¨Con calma flor de campo, te explicare de forma detallada una serie de tecnicas que puedes seguir para poder detectar los errores en tu codigo de dataframe ... (genera un texto detalllado sin ser tan largo) ¨ |


<img width="620" height="603" alt="image" src="https://github.com/user-attachments/assets/9f61e803-0a3d-4620-9bb0-14c318802059" />

