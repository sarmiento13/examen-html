**Documento Técnico: Examen Práctico de HTML Semántico (Actualizado)**
**Cargo:** Jose Luis Alvarez Escobar / Docente-APSTI
**Objetivo:** Evaluar HTML semántico, estructura de proyectos, navegación y formularios.

---

### **1. Problema a Solucionar**

La startup **"EcoBook"** necesita un sitio web de 4 páginas para reservas de alojamientos ecológicos. Los alumnos deben desarrollarlo usando:

- **HTML semántico**.
- Estructura de proyecto organizada.
- Formulario funcional de registro.
- Navegación coherente.

---

### **2. Requerimientos Funcionales**

#### **Estructura del Proyecto**

```
📁 examen-html/
├── 📁 .github/workflows    (Ya creada no tocar)
├── 📁 assets/          (Imágenes/icons)
├── 📁 css/             (Estilos)
├── 📁 js/              (Opcional, para validación de formulario)
├── 📁 pages/
│   ├── alojamientos.html
│   ├── contacto.html
│   └── registro.html   <!-- Nueva página -->
└── index.html
```

#### **Páginas y Contenido**

**a) `index.html` (Inicio)**

- `<header>`: Logo + menú de navegación (`<nav>`) con links a **todas las páginas**.
- `<main>`:
  - `<article>`: Introducción a EcoBook (texto + imagen).
  - `<section>`: 2 alojamientos destacados (cards con `<figure>`).
- `<footer>`: Enlaces a "Contacto" y "Registro".

**b) `alojamientos.html` (Listado)**

- Tabla (`<table>`) con: Nombre, Ubicación, Precio/noche.
- `<aside>`: "Tips eco-friendly" (lista desordenada `<ul>`).

**c) `contacto.html`**

- Formulario (`<form>`) con: Nombre, Email, Mensaje (`<textarea>`).
- `<address>`: Info ficticia (ej: "contacto@ecobook.com").

**d) `registro.html` (Nueva página)**

- Formulario de registro con los **siguientes campos**:
  - Nombre completo (`<input type="text">`).
  - Email (`<input type="email">`).
  - Contraseña (`<input type="password">`).
  - Checkbox: "Acepto términos y condiciones" (`<input type="checkbox">`).
  - Botón: "Registrarme" (`<button type="submit">`).

---

### **3. Requerimientos No Funcionales**

- **HTML Semántico:**
  - Uso obligatorio de `<main>`, `<section>`, `<article>`, `<footer>`, etc.
  - **Prohibido:** `<div>` para secciones clave.
- **Formulario de Registro:**
  - Campos con atributos `required` y `placeholder`.
  - Estructurado con `<fieldset>` y `<legend>` ("Datos de usuario").
- **Accesibilidad:**
  - Etiquetas (`<label>`) asociadas a cada input.
  - Texto alternativo en imágenes.
- **Navegación:** Links deben funcionar entre todas las páginas.

---

### **4. Criterios de Evaluación (Actualizados)**

| **Aspecto** | **Puntaje** |
| --- | --- |
| Estructura de proyecto | 15% |
| HTML semántico | 25% |
| Formulario de registro | 25% |
| Navegación y contenido | 20% |
| Accesibilidad y validación | 15% |

**Nota mínima aprobatoria:** 70/100.

---

### **5. Observaciones**

- ⚠️ **Penalización:** Uso de `<div>` en lugar de etiquetas semánticas (-5% por cada caso).

**📌 Nota final:** El formulario de registro debe ser **100% funcional en HTML** (no se requiere backend, pero sí estructura válida).

### **6. Pasos para rendir el examen**
1. Haz **fork** de este repositorio
```bash
https://github.com/IESTP-JMA/examen-html
```
3. Clona el repositorio
4. Ingresa a la carpeta clonada
2. Comienza por crear la estructura del proyecto
3. Completa los archivo HTML  segúm ñps requitos del Examen
4. Sube tus cambios con `git push`
5. Revisa los resultados en la pestaña **"Actions"** de tu repo
