# AgendaYa (EBP08) — Plataforma de Reserva de Servicios

Bienvenido a la organización oficial de **AgendaYa**, un proyecto desarrollado en la fábrica-escuela **CodeF@ctory** para la materia Análisis y Diseño de Sistemas II (AYD2) de la **Universidad de Antioquia**.

---

## 🎯 Sobre el Proyecto

**AgendaYa** es una plataforma web centralizada diseñada para optimizar el proceso de agendamiento y reserva de citas en empresas de servicios (salones de belleza, centros de salud, campos deportivos, entre otros). Permite a los clientes buscar negocios por ubicación y servicio, consultar disponibilidad en tiempo real y confirmar reservas sin riesgo de sobreventa o cruce de horarios.

---

## 👥 Equipo de Desarrollo 

* **Oscar Plaza** — Backend, Base de Datos, Integración y Despliegue.
* **Karen Vergara** — Backend, Modelado Comercial y Base de Datos (Supabase).
* **Arelis Giraldo** — Backend, Modelo de Proveedores y Despliegue Frontend (Vercel).
* **Karelyn Caicedo** — Backend, Módulo Geográfico, Disponibilidad y Despliegue (Render).
* **Ana Mora y Equipo** — Análisis 1, Prototipado y Diseño Frontend Inicial.
* **Santiago Echeverri** - Análisis 1, Construcción Historias de usuario en UHM.
* **Samuel Seguro** - Análisis 1, Gestion AzureDevops
* **Cristian Arias** - Análisis 1, Gestion AzureDevops
* **Alejandro Chavarria** - Gestion
* **Felipe Uribe** - Gestion

---

## 🔄 Metodología de Trabajo

El proyecto se gestiona mediante la metodología ágil **Scrum** en 3 iteraciones (sprints), aplicando la estrategia de flujo de trabajo **Trunk-based development**:
* Rama principal protegida (`main` / `Develop`).
* Integración continua mediante Pull Requests con al menos 1 aprobación obligatoria de revisión por pares.

---

## 🗺️ Hoja de Ruta (Sprints)

### 🟢 Sprint 1 (Completado — 22 de Septiembre, 2026)
* **Backend:** Modelo relacional completo (`Departamento`, `Municipio`, `Servicio`, `Proveedor`, `ServicioProveedor`, `Disponibilidad`, `Reserva`). API REST de búsqueda combinada y agendamiento con prevención de choques de horario (HTTP 409).
* **Frontend:** Interfaz web completa integrada con la API real mediante un patrón adaptador.
* **Despliegue Cloud:** Supabase (PostgreSQL) $\rightarrow$ Render (Backend Java 21) $\rightarrow$ Vercel (Frontend React).

### 🟡 Sprint 2 (Planeado)
* Incorporación de la entidad `Profesional` con agendas individuales por empleado.
* Panel de administración para proveedores (`ADMIN_PROVEEDOR`) para confirmar o cancelar citas.
* Ajuste de actualización automática del estado de `Disponibilidad` al agendar.

### 🔵 Sprint 3 (Planeado)
* Módulo de autenticación de usuarios con control de acceso basado en roles (Cliente, Admin Proveedor, Profesional, Admin Plataforma).
* Gestión de perfiles de usuario y notificaciones por correo electrónico.

---

## 🔗 Repositorios del Proyecto

* [📦 Repositorio Backend (Spring Boot + Java 21)](https://github.com/EBP08-Reserva-de-Servicios/Backend)
* [💻 Repositorio Frontend (React + TypeScript)](https://github.com/EBP08-Reserva-de-Servicios/Frontend)
* [🌐 Aplicación en Producción (Vercel)](https://frontend-arelisgiraldo.vercel.app)
