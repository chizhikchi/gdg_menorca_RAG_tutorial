# 🏨 RAG Hotel Assistant - Tutorial Básico

**Tutorial básico** para familiarizarse con **RAG (Retrieval-Augmented Generation)** usando **Vertex AI** y **Gemini**. Este repositorio contiene una introducción práctica en dos partes para entender las **bases de la construcción de sistemas RAG** con la **SDK de Python de Vertex AI**.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/chizhikchi/gdg_menorca_RAG_tutorial/blob/main/generate_hotel_info.ipynb)
[![Python 3.9+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Vertex AI](https://img.shields.io/badge/Powered%20by-Vertex%20AI-4285f4.svg)](https://cloud.google.com/vertex-ai)

---

## 📖 Descripción

Este **tutorial básico** te enseña los **fundamentos de RAG** y cómo construir tu primer sistema paso a paso usando la **SDK de Python de Vertex AI**. Ideal para familiarizarse con los conceptos y herramientas esenciales antes de proyectos más avanzados.

### 🎯 **Objetivo del Tutorial**
- Entender **qué es RAG** y cómo funciona
- Aprender las **bases de construcción** en Vertex AI
- Practicar con un **caso de uso simple** (asistente hotelero)
- Familiarizarse con la **SDK de Python** de Google Cloud

### ✨ Características

- 📚 **Tutorial paso a paso** para principiantes
- 🔧 **Fundamentos prácticos** de RAG con Vertex AI
- 💻 **SDK de Python** explicada desde cero
- 🏨 **Caso de uso simple** y comprensible
- 🎨 **Interfaz básica** con Gradio

---

## 📁 Estructura del Proyecto

```
📦 gdg_menorca_RAG_tutorial/
├── 📓 generate_hotel_info.ipynb     # Notebook 1: Generación de documentos
├── 📓 rag_tutorial.ipynb            # Notebook 2: Tutorial RAG completo
├── 🗂️ hotel_chatbot_documents.json  # Archivo con los prompts de referencia 
├── 📖 README.md                     # Este archivo
└── 📸 slides.pdg                    # Los slides que utilicé en el taller
```

---

## 🚀 Tutorial Básico en 2 Partes

### 📓 **Parte 1: Generación de Documentos**
**Archivo:** `generate_hotel_info.ipynb`

Para montar un chatbot basado en RAG lo primero que necesitamos son datos. 
Dado que este taller fue preparado para un evento que se celebró en Menorca los días 28 y 29 de julio de 2025, 
el caso de uso que se me ocurrió es un chatbot que facilita el acceso a la información sobre un hotel.

Puedes elegir entre usar el `hotel_chatbot_documents.json` para generar el corpus, 
coger unos archivos .txt que ya tengas o crear un `.json` del mismo formato con tus propios prompts. 

**Fundamentos que aprenderás:**
- ✍️ Uso básico de la API de Gemini
- 💾 Manejo de archivos en Google Drive desde Colab
- 🔧 Estructuración de prompts para generación de contenido
- 📝 Preparación de documentos para RAG

**Duración:** ~15 minutos | **Nivel:** Principiante

### 📓 **Parte 2: Construcción del Sistema RAG**
**Archivo:** `rag_tutorial.ipynb`

**Fundamentos que aprenderás:**
- 📚 **Conceptos básicos** de RAG: ¿qué es y para qué sirve?
- 🛠️ **SDK de Vertex AI**: creación de corpus y carga de documentos
- 🔍 **Retrieval**: cómo el sistema busca información relevante
- 🤖 **Generation**: cómo se genera la respuesta final
- 🎨 **Interfaz simple** con Gradio para probar el sistema

**Duración:** ~25 minutos | **Nivel:** Principiante

---

## ⚡ Inicio Rápido

### 1️⃣ **Requisitos Previos**

- Cuenta de **Google Cloud** con facturación activada
- **Vertex AI API** habilitada en tu proyecto
- Clave API de **Gemini** ([Obtener aquí](https://aistudio.google.com/app/apikey))

### 2️⃣ **Configuración de Secretos en Colab**

Antes de ejecutar los notebooks, configura estos secretos en Google Colab (🔑):

| Nombre del Secreto | Descripción | Ejemplo |
|-------------------|-------------|---------|
| `PROJECT_ID` | ID de tu proyecto de Google Cloud | `mi-proyecto-123456` |
| `GEMINI_API_KEY` | Clave API de Gemini | `AIza...` |

### 3️⃣ **Ejecución**

1. **Abre el Notebook 1** en Google Colab: `generate_hotel_info.ipynb`
   - Configura las rutas al `.json` y al directorio donde quieras que se guarden los archivos generados
   - Genera la documentación del hotel

2. **Abre el Notebook 2** en Google Colab: `rag_tutorial.ipynb`
   - Crea el sistema RAG
   - Lanza la interfaz de chat

¡Listo! 🎉

---

## 📚 Fundamentos que Aprenderás

### 🧠 **Conceptos Básicos de RAG**
- **¿Qué es RAG?** Diferencia entre generación pura y aumentada
- **¿Cómo funciona?** El flujo: Retrieval → Augmentation → Generation

### 🛠️ **SDK de Python - Vertex AI**
- **Configuración básica** de cliente y proyecto
- **Manejo de corpus**: creación, configuración y gestión
- **Carga de documentos**: desde archivos locales y Drive
- **Modelos generativos**: integración con herramientas RAG

### 💡 **Fundamentos Prácticos**
- **Embeddings**: cómo se vectorizan los documentos
- **Búsqueda semántica**: encontrar información relevante
- **Construcción de respuestas**: combinar contexto + pregunta
- **Interfaz básica**: mostrar resultados al usuario

---

## 🎯 Ideal Para

Este tutorial básico es perfecto para:

- 🎓 **Principiantes en RAG** que quieren entender los fundamentos
- 👨‍💻 **Desarrolladores** nuevos en Vertex AI y su SDK de Python
- 🏢 **Profesionales** que necesitan evaluar la viabilidad de RAG
- 📚 **Estudiantes** aprendiendo sobre IA generativa aplicada

## 🆘 Soporte y Preguntas

### ❓ **Preguntas Frecuentes**

**P: ¿Necesito conocimientos previos de IA?**
R: No, el tutorial está diseñado para principiantes.

**P: ¿Cuánto cuesta ejecutar este tutorial?**
R: Los costos son mínimos (~$1-2 USD) para las pruebas básicas.

**P: ¿Puedo usar otros documentos además de los del hotel?**
R: ¡Absolutamente! Puedes adaptar el sistema para cualquier dominio.

### 💬 **¿Necesitas ayuda?**

- 📧 Email: [mándame un correo](mailto:chizhikchi@gmail.com)
- 💬 LinkedIN: [¡conectemos!](https://www.linkedin.com/in/mariia-chizhikova/)

---

## 🌟 Agradecimientos

- **Google Cloud** por Vertex AI y las herramientas de IA
- **Google Colab** por el entorno de desarrollo gratuito
- **Gradio** por hacer las interfaces web tan sencillas
- **Comunidad de desarrolladores** por el feedback y contribuciones

---

<div align="center">

### ⭐ ¡Si te gusta este proyecto, dale una estrella! ⭐

**Hecho con ❤️ para la comunidad de IA en español**

[🚀 Empezar Tutorial](generate_hotel_info.ipynb)

</div>