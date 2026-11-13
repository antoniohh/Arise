# Release v1.4.1 — Incorporación de Cáceres en el Foco y Renovación Multimedia

**Fecha:** 13 de Noviembre de 2026  
**Versión:** 1.4.1  

## Resumen de la Versión

Esta versión menor incorpora el nuevo proyecto **Cáceres en el Foco** en el CV tras *Voltio*, junto con la actualización y sustitución de un conjunto de capturas de previsualización en formato WebP de alta fidelidad para los proyectos principales del portfolio.

---

## 🚀 Proyectos Incorporados

1. **Cáceres en el Foco (`servicios.hoy.es/caceresenelfoco`)**:
   - Landing interactiva y pasarela de redirección oficial para el concurso fotográfico organizado por Diario HOY con motivo del 40º Aniversario de Cáceres como Patrimonio de la Humanidad por la UNESCO.
   - Cuenta con pasarela de enlace a campañas en Qualifio (`/inscripcion/`, `/subir/`, `/galeria/`), gestión de 5 fases de concurso vía `config.json`, temporizador en tiempo real con cuenta atrás y panel administrativo protegido con control manual y por calendario.
   - Stack: Web, PHP, JavaScript, CSS.
   - Enlaces: Despliegue en producción y repositorio GitHub (`antoniohh/CaceresFoco`).

---

## 🖼️ Multimedia y Optimización de Assets

- **Nuevas imágenes de proyecto (WebP 1280×720)**:
  - `public/img/caceresfoco.webp`: Captura optimizada de la landing del concurso fotográfico.
  - Actualización y sustitución de previsualizaciones en:
    - `aimos.webp`
    - `arise.webp`
    - `audihoy.webp`
    - `brody.webp`
    - `combustible.webp`
    - `embalses.webp`
    - `glucoluna.webp`
    - `hooper.webp`
    - `kronos.webp`
    - `luz.webp`
    - `newspaint.webp`
    - `padme.webp`
    - `tuanbyte.webp`

---

## ⚙️ Control de Versiones y Verificación

- Actualización de versión a **1.4.1** en `package.json`, `package-lock.json`, `README.md` y `AGENTS.md`.
- Verificación de tipos y compilación completa mediante `astro check && astro build` (0 errores, 0 warnings).
