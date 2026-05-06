# 🌍 Gestor de Países — CRUD Sumativa 4

Aplicación web construida con **React + Vite** para gestionar una lista de países usando datos en tiempo real desde la API [REST Countries](https://restcountries.com).

---

## 🚀 Funcionalidades

- 📋 **Listar** países con bandera, nombre y continente
- ➕ **Agregar** países consultando la API automáticamente
- ✏️ **Editar** un país (realiza nueva consulta a la API)
- 🗑️ **Eliminar** países con confirmación
- 🔒 **Validaciones** de negocio:
  - Máximo **16 países** en total
  - Máximo **4 países por continente**
  - **Sin duplicados**
- 💾 **Persistencia** con `localStorage` (los datos se mantienen al recargar)
- 📊 **Estadísticas** en tiempo real: total de países, espacios disponibles y continentes representados

---

## 🗂️ Estructura del Proyecto

```
crud-paises-app/
├── index.html
├── package.json
├── vite.config.js
└── src/
    ├── main.jsx          # Punto de entrada de React
    ├── App.jsx           # Controlador principal y manejo de vistas
    ├── index.jsx         # Vista principal — tabla de países
    ├── views/
    │   └── Form.jsx      # Vista del formulario — agregar/editar
    └── css/
        └── styles.css    # Estilos personalizados
```

---

## ⚙️ Instalación y uso

```bash
# 1. Instalar dependencias
npm install

# 2. Iniciar en modo desarrollo
npm run dev

# 3. Abrir en el navegador
http://localhost:5173
```

---

## 🌐 API utilizada

**REST Countries** — `https://restcountries.com/v3.1/name/{nombre}`

El sistema busca el país por nombre exacto y extrae automáticamente:
- Nombre oficial (`name.common`)
- Continente (`continents[0]`)
- Bandera (`flags.svg`)

> Los nombres deben ingresarse en **inglés o español exacto** (ej: `Germany`, `Chile`, `France`).

---

## 🎯 Reglas del sistema

| Regla | Detalle |
|---|---|
| Máximo total | 16 países |
| Máximo por continente | 4 países |
| Duplicados | No permitidos |
| Nombre | Debe ser exacto (inglés o español) |

---

## 🖼️ Tecnologías

| Tecnología | Uso |
|---|---|
| React 18 | UI y manejo de estado |
| Vite 4 | Bundler y servidor de desarrollo |
| Bootstrap 5 | Estilos y componentes visuales |
| Bootstrap Icons | Íconos |
| REST Countries API | Datos de países en tiempo real |
| localStorage | Persistencia de datos |

---

## 👨‍💻 Autor

**MaTi**  
Estudiante de Programación Front-End  
— Evaluación Sumativa 4

---

## 📄 Licencia

Proyecto de uso educativo — sin licencia comercial.
