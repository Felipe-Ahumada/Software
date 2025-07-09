# 🛂 Sistema de Declaraciones Aduaneras – Paso Los Libertadores

## 📘 Documentación de Arquitectura y Prototipado

Este repositorio contiene el Documento de Arquitectura del Sistema (DAS V5) y la tercera entrega de la presentación del caso "Aduanas", orientado a digitalizar el control de salida terrestre entre Chile y Argentina.

---

## 🎯 Objetivo del Proyecto

Reducir los tiempos de espera en frontera y modernizar el proceso de control de salida mediante:

- Digitalización de formularios de salida de vehículos, productos y mascotas.
- Validación automática de documentos.
- Interoperabilidad con SAG, PDI, Registro Civil y Aduana Argentina.
- Plataforma web segura y accesible para ciudadanos y funcionarios.

---

## 🏗️ Arquitectura del Sistema

- **Estilo:** Monolítico multicapa
- **Tecnologías:** Spring Boot, PostgreSQL, HTML/CSS/JS, RESTful APIs
- **Capas:**
  - Presentación (Web)
  - Lógica de Negocio
  - Persistencia de Datos
  - Integración Externa

---

## 🧩 Modelo 4+1 aplicado

- **Vista de Escenario:** Diagramas de casos de uso para ciudadanos y fiscalizadores.
- **Vista Lógica:** Clases como `Usuario`, `FormularioSalidaVehiculo`, `DocumentoAdjunto`.
- **Vista de Desarrollo:** Organización modular por controladores, servicios, repositorios.
- **Vista de Procesos:** Flujo del registro, validación y auditoría.
- **Vista Física:** Despliegue centralizado cliente-servidor con integración a APIs externas.

---

## ✅ Funcionalidades Clave

### Para Ciudadanos
- Registro y login
- Formularios digitales para:
  - Vehículos (con padrón, seguro y permiso notarial si aplica)
  - Productos no equipaje
  - Mascotas (CZE)
- Seguimiento de estado y edición de formularios

### Para Funcionarios
- Panel de validación con filtros
- Revisión de formularios y documentos
- Acceso a integraciones externas
- Registro de acciones para trazabilidad

---

## 🎨 Diseño de Prototipos

- **Herramienta:** Figma (colaborativa, en la nube)
- **Propósito:** Validar experiencia de usuario antes del desarrollo
- **Componentes diseñados:**
  - Panel de ciudadano
  - Formularios digitales
  - Panel de revisión del funcionario
  - Estado de solicitudes y filtros

---

## 🧪 Evaluación de Usabilidad

- **Heurísticas de Nielsen evaluadas:**
  - ✔ Visibilidad del estado del sistema
  - ✔ Prevención de errores
  - ✔ Consistencia visual
  - ✘ Ayuda y documentación (a mejorar)
- **Resultado:** 9 de 10 cumplidas. Mejora iterativa en documentación planificada.

---

## 🛠 Control de Versiones

- **Herramienta:** Git + GitHub
- **Estrategia:** Versionado semántico (MAJOR.MINOR.PATCH)
- **Ventajas:**
  - Claridad en cambios
  - Mejora la colaboración
  - Facilita integración continua (CI/CD)

---

## 🏁 Conclusión

Este sistema aborda una necesidad nacional crítica al modernizar el control fronterizo. A través de una arquitectura sólida, diseño centrado en el usuario y herramientas modernas de desarrollo, se garantiza una solución eficiente, segura y escalable que mejora tanto la experiencia ciudadana como el control institucional.

---

## 👥 Autores

- Felipe Ahumada Silva  
- Francisca Barrera  
- Patricio Zapata  
- Emmanuel Opazo
