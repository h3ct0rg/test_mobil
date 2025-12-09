# 📱 Prueba Técnica — Android Mobile Developer  
**Stack requerido:** Kotlin · Jetpack Compose · MVVM + Clean Architecture · Retrofit · OkHttp · Room · Hilt · Coroutines · Flow

Esta prueba está diseñada para evaluar las habilidades principales de un **Android Developer Semi Senior**, cubriendo arquitectura, buenas prácticas, consumo de APIs, persistencia local, manejo de estados, asincronía y uso adecuado del ecosistema moderno de Android.

El proyecto puede completarse en **4 a 6 horas**.

---

# 🎯 Objetivo General  
Construir una pequeña app Android en **Kotlin + Jetpack Compose**, con una arquitectura **MVVM + Clean Architecture**, que consuma una API pública, almacene datos localmente con Room, y presente los datos en pantalla mediante Compose.

---

# 🧩 1. Funcionalidad Principal

### ✔️ Requerimiento  
Crear una app que muestre una lista de **usuarios** obtenidos desde la API pública:
ejem: https://jsonplaceholder.typicode.com/users


### 📱 Pantallas requeridas

#### 1. 📄 Lista de Usuarios
- Mostrar nombre, email y ciudad.
- Debe ser una pantalla hecha 100% en **Jetpack Compose**.
- El usuario debe poder refrescar los datos con un **pull-to-refresh**.

#### 2. 👤 Detalle de Usuario
- Al presionar un usuario, se abre una pantalla de detalle mostrando:
  - Nombre  
  - Email  
  - Teléfono  
  - Website  
  - Ciudad  
  - Compañía  

### ⭐ Requisitos técnicos obligatorios

- Arquitectura **MVVM + Clean Architecture**
- Inyección de dependencias con **Hilt**
- Networking usando **Retrofit + OkHttp**
- Lógica asincrónica usando **Coroutines + Flow**
- Persistencia de datos con **Room**
  - Guardar localmente la lista de usuarios
  - Usar los datos locales cuando no haya internet
- Manejo adecuado de estados en Compose:
  - Cargando
  - Error
  - Contenido

---

# 🧩 2. Estructura del Proyecto

La app debe organizarse bajo una arquitectura limpia, con las siguientes capas:
/domain
/model
/repository
/usecases

/data
/remote (Retrofit)
/local (Room)
/repository (implementación)

/ui
/list
/detail
/components


---

# 🧩 3. Requerimientos Técnicos Específicos

### 🔹 Retrofit + OkHttp
- Implementar interceptor de logging.
- Manejo simple de errores (400–500).

### 🔹 Room
- Entidad `UserEntity`.
- DAO con operaciones básicas:
  - insertAll
  - getAll
  - clear

### 🔹 Coroutines + Flow
- Debe usarse Flow en el repository para emitir estados.
- ViewModel debe exponer StateFlow o MutableStateFlow.

### 🔹 Jetpack Compose
- Uso de `LazyColumn`
- Uso de `Scaffold`
- Estado gestionado correctamente (no en la UI)
- No usar Fragments

---

# 🧪 Puntos Extra (Opcionales)

Estos puntos no son obligatorios, pero suman mucho a la evaluación:

### ⭐ Dark Mode implementado correctamente  
### ⭐ Animaciones simples en Compose  
### ⭐ Tests unitarios en ViewModel  
### ⭐ Manejo offline-first más robusto  

---

# 🧩 4. GitHub Flow (Obligatorio)

1. Crear una rama siguiendo esta convención:
feature/<nombre-del-candidato>


2. Commits pequeños y descriptivos.  
3. Al finalizar, abrir un **Pull Request** hacia `main`.  
4. Incluir instrucciones mínimas para correr el proyecto.

---

# 📦 Entregables

El candidato debe entregar:

- Proyecto Android completo
- Código organizado bajo Clean Architecture
- Pantallas en Jetpack Compose
- Uso de Retrofit, Room, Hilt y Flow
- Pull Request en GitHub

---

# ⏱️ Tiempo estimado  
**4 a 6 horas máximo**

---

# 🏁 Criterios de Evaluación

| Área | Peso |
|------|------|
| Kotlin + buenas prácticas | ⭐⭐⭐⭐ |
| Jetpack Compose | ⭐⭐⭐⭐ |
| MVVM + Clean Architecture | ⭐⭐⭐⭐ |
| Networking + Retrofit | ⭐⭐⭐ |
| Manejo de estado en Compose | ⭐⭐⭐⭐ |
| Room + persistencia | ⭐⭐⭐ |
| Coroutines + Flow | ⭐⭐⭐ |
| Git (commits + PR) | ⭐⭐⭐⭐ |
| Extra: Dark Mode, animaciones, tests | ⭐⭐ |

---

# 🙌 Notas Finales  
El objetivo no es complejidad, sino **calidad**, **orden**, y un buen manejo del ecosistema moderno de Android.



