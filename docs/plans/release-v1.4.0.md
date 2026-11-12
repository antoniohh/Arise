# Release v1.4.0 — Actualización de Proyectos, Multimedia y Reorganización de CV

**Fecha:** Noviembre 2026  
**Versión:** 1.4.0  

## Resumen de la Versión

Esta versión representa una actualización integral del contenido del portafolio/CV personal, incorporando nuevos desarrollos web, plataformas editoriales y utilidades técnicas desplegadas en producción, junto con una completa optimización de assets visuales a formato WebP.

---

## 🚀 Proyectos Incorporados

1. **Tuanbyte (`tuanbyte.es`)**: Landing interactiva y catálogo estilo ferretería para el taller y canal de mecánica, bricolaje y tecnología (Astro + Tailwind CSS).
2. **Luz Extremadura (`luz.antoniohorrillo.com`)**: Aplicación web SPA para la consulta en tiempo real del precio regulado de la luz PVPC 2.0TD con semáforo energético y previsión (Astro + Tailwind CSS + Chart.js).
3. **Combustible Extremadura (`combustible.antoniohorrillo.com`)**: Monitorización de precios de Gasolina 95 y Diésel en los 179 municipios de Extremadura (Astro + Tailwind CSS + Chart.js).
4. **GlucoLuna (`glucoluna.antoniohorrillo.com`)**: Herramienta de salud para registro de glucosa, dosis nocturna y guía visual de pinchazo con pluma (Astro + Tailwind CSS + Lucide).
5. **Embalses de Extremadura (`embalses.antoniohorrillo.com`)**: Consulta del estado hídrico de los 42 embalses autonómicos con datos oficiales del MITECO (Astro + React + Tailwind CSS).
6. **Brody**: Plataforma editorial para la redacción y distribución del Diario HOY con optimización SEO/AEO/GEO asistida por Google GenAI (Slim 4 + React 19 + Tailwind CSS + SQLite).
7. **AudiHOY**: Panel de control analítico de audiencias y redes sociales para Diario HOY integrando GFK (DAM) y Adobe Analytics (Slim 4 + React 18 + Tailwind CSS).

---

## 🔄 Actualizaciones y Correcciones

- **Hooper**: Corrección del nombre en el CV (anteriormente *Hoper*), reflejando su evolución a v1.7.0 con soporte React 19, Symfony, WebCodecs y PHP 8.4.
- **NewsPaint & Aimos**: Renovación de capturas de pantalla de la suite editorial v5.0.
- **Voltio**: Mantenimiento del proyecto histórico junto a la nueva aplicación abierta Luz Extremadura.
- **Retirada de Blog**: Se elimina la entrada del blog para priorizar los proyectos web y landings independientes.
- **Reordenación de Proyectos**: Se priorizan los proyectos activos e independientes en cabecera:
  1. Arise
  2. Tuanbyte
  3. YouTube Channel
  4. Fulcrum
  5. Luz Extremadura
  6. Combustible Extremadura
  7. GlucoLuna
  8. Embalses de Extremadura
  9. Hooper
  10. Brody
  11. NewsPaint
  12. AudiHOY
  13. Aimos
  14. Padme
  15. Voltio ... y continuaciones.

---

## 🖼️ Multimedia y Optimización de Assets

- Conversión de 11 capturas PNG de alta resolución a formato `.webp` optimizado a 1280×720 (16:9), alojadas en `public/img/`.
- Limpieza de imágenes temporales de la raíz del repositorio.

---

## ⚙️ Cambios Técnicos y Tipado

- Actualización de `src/cv.d.ts` con propiedades opcionales `image?: string` y `url?: string` en la interfaz `Projects`.
- Build verificado con `astro check && astro build` (0 errores, 0 warnings).
