# 📘 Documento de Arquitectura de Software (DAS)
## Proyecto: Sistema de Declaración Aduanera - Paso Internacional Los Libertadores

### 🗂️ Versión 1.0 | Última revisión: 29/05/2025

---

## 🧩 Descripción General

Este documento detalla la arquitectura del sistema informático desarrollado para modernizar el control fronterizo terrestre en el Paso Internacional Los Libertadores. La propuesta responde a la necesidad de digitalizar los procesos manuales asociados a la salida de vehículos, productos y mascotas desde Chile hacia Argentina, mejorando la eficiencia, trazabilidad y experiencia del usuario.

---

## 🎯 Objetivo

Diseñar e implementar un sistema monolítico multicapa que permita:
- Declaración anticipada digital por parte del ciudadano.
- Validación automatizada por funcionarios de Aduanas.
- Integración con sistemas externos (SAG, PDI, Registro Civil, Aduana Argentina) vía APIs REST.

---

## 🏗️ Arquitectura del Sistema

- **Estilo:** Monolítico Multicapa
- **Capas principales:**
  - Presentación (HTML, CSS, JS)
  - Lógica de negocio (Spring Boot – Java)
  - Acceso a datos (PostgreSQL)
  - Integración externa (consumo de APIs REST)

- **Clientes del sistema:**
  - Ciudadano (Web/Móvil)
  - Agente Aduanero (Estación de trabajo)
  - Jefe de Turno (Auditoría y trazabilidad)

- **Servicios externos consumidos:**
  - Registro Civil (validación padrón)
  - PDI (estado migratorio)
  - SAG (CZE mascotas)
  - Aduana Argentina (historial vehicular)

---

## 🧑‍💻 Principales Funcionalidades

### Para el Ciudadano
- Registro seguro y autenticación
- Formulario digital de:
  - Vehículos
  - Productos no equipaje
  - Mascotas (CZE)
- Adjuntar documentos (PDF/JPG)
- Consulta de estado, edición y reenvío

### Para el Funcionario de Aduanas
- Panel de revisión con filtros
- Validación de formularios y documentos
- Integración con sistemas externos
- Aprobación, rechazo o estado pendiente

---

## 🛠️ Patrones y Principios de Diseño

- **Modelo Vista Controlador (MVC)**
- **Repository Pattern**
- **Control de Acceso por Rol**
- **Encapsulación, Cohesión, Bajo Acoplamiento, Modularidad**

---

## 📐 Modelo 4+1 y Vistas

- **Vista de Escenario:** Casos de uso ciudadanos y validaciones
- **Vista Lógica:** Clases: Usuario, Formulario, Vehículo, Documento
- **Vista de Desarrollo:** Controladores, Servicios, Repositorios
- **Vista de Procesos:** Flujo del formulario desde ingreso hasta validación
- **Vista Física:** Cliente web ↔ Servidor backend ↔ DB + APIs externas

---

## 📈 Requisitos de Calidad

| Atributo        | Evaluación                                       |
|-----------------|--------------------------------------------------|
| Usabilidad      | Formularios intuitivos, pruebas con usuarios     |
| Accesibilidad   | Cumplimiento WCAG 2.1 AA                         |
| Bajo Acoplamiento | Módulos independientes para validaciones        |
| Alta Cohesión   | Cada módulo cumple una función única             |
| Encapsulación   | APIs externas ocultas al usuario final           |

---

## ✅ Conclusión

El sistema propuesto permite al Estado avanzar hacia una Aduana moderna, eficiente y conectada. Se estructura en base a principios de diseño sólidos y un enfoque arquitectónico coherente con el entorno institucional, priorizando la trazabilidad, seguridad y experiencia ciudadana.

---

## 👤 Autores

- Felipe Ahumada Silva  
- Francisca Barrera  
- Patricio Zapata

---

## 📚 Referencias

- Booch, G. et al. (2005). UML. Addison-Wesley.  
- Sommerville, I. (2011). Ingeniería del Software. Pearson.  
- Nielsen, J. (1993). Usability Engineering. Morgan Kaufmann.  
- W3C. (2018). WCAG 2.1: https://www.w3.org/TR/WCAG21/  
- DUOC UC (2024). Apuntes RQY1102.

