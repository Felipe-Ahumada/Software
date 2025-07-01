# Sistema de Modernización Aduanera - Paso Internacional Los Libertadores

## 🛂 Descripción del Proyecto

Este proyecto tiene como objetivo principal digitalizar, automatizar y optimizar el proceso de control aduanero terrestre chileno en el Paso Internacional Los Libertadores. El sistema está diseñado para permitir declaraciones anticipadas por parte de ciudadanos que viajan desde Chile hacia Argentina, facilitando los trámites de salida de vehículos, productos no considerados equipaje y mascotas.

## 🧩 Arquitectura del Sistema

- **Tipo de arquitectura:** Monolítica multicapa
- **Tecnología base:** Spring Boot (Java)
- **Capas:**
  - Presentación (Web UI para ciudadanos y funcionarios)
  - Lógica de negocio (validaciones, reglas, gestión)
  - Acceso a datos (Base de datos relacional)
  - Integración externa (APIs: SAG, PDI, Registro Civil)

## 👥 Actores del Sistema

- **Ciudadano Saliente:** Registra formularios y adjunta documentos.
- **Funcionario de Aduana:** Revisa, valida y responde formularios.
- **Jefe de Turno:** Supervisa el flujo y accede a reportes.
- **Sistemas externos:** SAG, PDI y Registro Civil (consumo vía API REST).

## 📋 Funcionalidades Clave

### Ciudadano
- Registro y autenticación.
- Completar formularios de:
  - Salida de vehículos
  - Transporte de productos no equipaje
  - Salida de mascotas (CZE)
- Adjuntar documentos (padrón, seguro, certificados)
- Consultar estado de las solicitudes.

### Funcionario
- Revisión de formularios con filtros.
- Validación automática/manual de documentos.
- Aprobación, rechazo o marcación como pendiente con observaciones.

## 🧪 Requisitos

### Requisitos Funcionales
- Digitalización y gestión de formularios.
- Validación automática con APIs externas (SAG, PDI, Registro Civil).
- Autenticación de usuarios.
- Trazabilidad completa del proceso.

### Requisitos No Funcionales
- Usabilidad (interfaz clara, intuitiva, accesible).
- Seguridad (control de acceso y protección de datos).
- Accesibilidad (cumplimiento de estándares WCAG).
- Eficiencia (respuestas rápidas del sistema).

## 🖼️ Prototipado

- **Herramienta usada:** Figma
- **Propósito:** Validar usabilidad, flujos y consistencia visual antes del desarrollo.
- **Mockups:** Formulario de salida, revisión de estado, vista de funcionario, historial, etc.

## ✅ Evaluación de Usabilidad

- **Método:** Heurísticas de Nielsen (10 principios)
- **Resultado:** 9 de 10 heurísticas cumplidas
- **Hallazgo crítico:** Falta de ayuda contextual/documentación visible.
- **Medidas tomadas:** Planificación de mejoras iterativas.

## 📁 Control de Versiones

- **Sistema de control:** Git + GitHub
- **Estrategia:** Versionado Semántico (`MAJOR.MINOR.PATCH`)
- **Repositorio:** [GitHub - Felipe Ahumada](https://github.com/Felipe-Ahumada/Software)
- **Ventajas:** Facilita colaboración, CI/CD, trazabilidad y manejo de ramas.

## 🧮 Gestión de Proyecto

- **Metodología:** Cascada
- **Fases completadas:**
  - Análisis de requerimientos
  - Diseño del sistema
  - Implementación (en curso)
  - Pruebas y despliegue (planificadas)
- **Carta Gantt:** Incluye planificación semanal, horas estimadas y responsables.

## 🏁 Conclusión

Este sistema representa un avance crítico en la modernización del proceso aduanero chileno, reduciendo los tiempos de espera en frontera, mejorando la interoperabilidad con otras entidades y optimizando la experiencia del ciudadano. Está alineado con los objetivos institucionales de eficiencia, transparencia y servicio de calidad.

---

© 2025 - Proyecto Aduanas | © 2025 – Felipe Ahumada, Francisca Barrera, Emmanuel Opazo, Patricio Zapata - DUOC UC
