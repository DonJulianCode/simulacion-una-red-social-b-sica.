# 🧠 Documentación de la Actividad: Red Social con Estructuras de Datos Avanzadas

## 1. Objetivo

Desarrollar un sistema conceptual en Python que simule una red social básica e integre el uso de las siguientes estructuras de datos: listas, tuplas, diccionarios, conjuntos, pilas, árboles y grafos. El propósito es demostrar su aplicación en la resolución de un problema concreto.

---

## 2. Estructura General del Proyecto

### 📁 Componentes principales

- **Base de Datos de Usuario:**  
  Estructurada mediante un diccionario (`usuarios`), donde cada clave representa el `username` y el valor es un diccionario que almacena `nombre`, `edad` y una `lista de amigos`.

- **Red de Conexiones (Grafo):**  
  Modelada como un grafo no dirigido usando:
  - Diccionarios anidados para lógica.
  - `NetworkX` para visualización y análisis estructural.

---

## 3. Aplicación de Estructuras de Datos

### 📌 Listas y Tuplas
- Uso de listas para representar amigos, historial, solicitudes, etc.
- Uso de tuplas para registrar datos inmutables, como el conjunto (username, edad).
- Se muestran ejemplos de slicing, indexación e inmutabilidad.

### 📌 Pilas (LIFO)
- Registro de actividades recientes de los usuarios.
- Se implementan funciones `registrar_actividad()` y `ver_actividades_recientes()` simulando `push` y `pop`.

### 📌 Colas (FIFO)
- Simulación de solicitudes de amistad pendientes en orden de llegada.
- Funciones `solicitar_amistad()` y `procesar_solicitud()` aplican `enqueue` y `dequeue`.

### 📌 Árboles
- Se implementa un árbol binario para agrupar usuarios por edad o tipo.
- Se utiliza para representar jerarquías y clasificaciones.

### 📌 Grafos
- La red de amigos es un grafo no dirigido.
- Se implementa lógica con diccionarios y visualización con `NetworkX`.
- Se permite agregar usuarios, conectar amigos, y representar la red.

---

## 4. Funciones Específicas

- `agregar_usuario(username, nombre, edad)`: agrega un nuevo usuario al sistema.
- `agregar_amigo(user1, user2)`: conecta a dos usuarios de forma bidireccional.
- `mostrar_estructura()`: imprime todos los usuarios y sus amigos en consola.
- `grafo_red_social()`: visualiza la red de conexiones utilizando NetworkX.

---

## 5. Comentarios y Estilo

Cada función está documentada con comentarios explicativos, que detallan su propósito, parámetros y efectos. Se utilizó estilo modular y nombres descriptivos para facilitar el mantenimiento y la lectura.

---

## 6. Justificación de Diseño

- Se priorizó la representación **explícita y visual** de las estructuras.
- Se eligió `NetworkX` por su potencia para visualizar grafos.
- Se trabajó con estructuras internas puramente en Python para respetar el enfoque conceptual del ejercicio.
