# ConectaTrabajo 🚧 (Work in Progress)

Plataforma web local diseñada para conectar a clientes con trabajadores independientes, prestadores de oficios y profesionales en la ciudad de Las Varillas. 

El objetivo principal es reducir la brecha digital local, centralizando la oferta de servicios independientes en una interfaz intuitiva y eficiente que permita a los trabajadores mostrar su experiencia y a los clientes encontrar soluciones de confianza rápidamente.

---

## 🛠️ Stack Tecnológico y Arquitectura

El ecosistema backend está desarrollado con tecnologías modernas y un enfoque estricto en la separación de responsabilidades:

* **Lenguaje y Framework:** Java 21 y Spring Boot 3 para un entorno robusto, eficiente y escalable.
* **Arquitectura:** Implementación del patrón arquitectónico Controller-Service-Repository para garantizar la modularidad y el desacoplamiento de la lógica de negocio y el diseño de REST APIs.
* **Seguridad:** Autenticación y autorización basada en roles (`ADMIN`, `TRABAJADOR`, `CLIENTE`) utilizando JSON Web Tokens (JWT) para proteger los endpoints críticos.
* **Buenas Prácticas:** Uso de Data Transfer Objects (DTO) siguiendo convenciones limpias de nomenclatura como `ProductoResponseDto` para el intercambio seguro y óptimo de información entre capas.

---

## 🌟 Características Principales (En Migración)

### 👥 Gestión de Roles y Autenticación
* Registro e inicio de sesión seguro mediante JWT diferenciando privilegios según el tipo de usuario.

### 🔨 Perfil del Trabajador
* Configuración de perfil profesional con fotografía, descripción detallada y datos de contacto seleccionables (WhatsApp, Instagram o ambos).
* Galería de fotos integrada para exhibir un portfolio de trabajos realizados con éxito.
* Asociación flexible a múltiples subcategorías de trabajo.

### 🔍 Sistema de Clasificación y Filtros Dinámicos
* Organización jerárquica de servicios: Categorías globales que agrupan múltiples subcategorías específicas para facilitar la navegación.
* Búsqueda avanzada y filtrado predictivo combinando localización por ciudad y especialidad de servicio.

### 💬 Reputación y Reseñas
* Sistema de feedback bilateral donde los clientes registrados pueden otorgar una puntuación (1 a 5) y dejar comentarios en el perfil de los trabajadores.
* Restricción de integridad: Lógica estricta en el backend que limita a una única reseña por cliente hacia un mismo trabajador para evitar fraudes en la reputación.

---

## 📈 Plan de Trabajo e Historial de Git

Esta versión (V2) representa una reescritura consciente y profesional a partir de un prototipo funcional previo. El desarrollo se gestiona bajo las siguientes directrices:

1. **Historias de Usuario (US):** Cada funcionalidad se desprende de un análisis previo de requisitos y criterios de aceptación.
2. **Conventional Commits:** El historial de Git sigue un estándar estricto (ej. `feat:`, `fix:`, `docs:`, `refactor:`) para asegurar la trazabilidad del código.
3. **Calidad de Código:** Enfoque en la clean arquitectura, legibilidad, consistencia en la nomenclatura y cobertura de pruebas unitarias.
