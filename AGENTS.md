# 🏗️ BokuNoData - Services Skeleton

## Resumen del Proyecto
Este repositorio es un **Skeleton** (esqueleto) diseñado para servir de base en proyectos que requieren una separación clara de responsabilidades. No contiene lógica de negocio final, sino la infraestructura necesaria para implementarla.

## Arquitectura (Clean Architecture)
El proyecto está dividido en dos grandes bloques para mantener un desacoplamiento total:
- **Backend:** Laravel (API / Reglas de Negocio).
- **Frontend:** Vue.js (Interfaz de Usuario / Cliente).

## Servicios Iniciales
- **AuthService:** Estructura base para el manejo de sesiones y seguridad.
- **Gateway:** Punto de entrada centralizado para la orquestación de datos.

## Definición de Agentes (Skeleton Mode)
*Este archivo sirve como placeholder para definir los futuros actores del sistema.*

1. **Agente Desarrollador:** Encargado de extender este esqueleto siguiendo los patrones de inyección de dependencias y repositorios.
2. **Agentes de Aplicación:** (A definir) Aquí se listarán los roles (Admin, API, Bot) una vez se implemente la lógica de dominio específica.

## Notas de Uso
- **Propósito:** Proveer un entorno listo para producción con una estructura de carpetas estandarizada.
- **Escalabilidad:** Cada nuevo servicio debe seguir el patrón de capas: `Domain` (Entidades), `Application` (Casos de Uso) e `Infrastructure` (Laravel/DB).