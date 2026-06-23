# Plan: Actualizar Astro de v4.3.2 a v7.0.2

## Resumen
Actualización mayor de Astro desde v4.3.2 hasta v7.0.2. Proyecto estático simple sin content collections, por lo que la migración debería ser directa.

## Requisitos previos
- [x] Node.js v22.23.0 (cumple requisito ^22.12.0)
- [x] Cambios recientes guardados en git

## Pasos del plan

### 1. Pre-actualización
- [x] Verificar que `npm run build` funciona correctamente
- [x] Crear backup del package.json actual

### 2. Actualizar dependencias
- [x] Ejecutar `npx @astrojs/upgrade` para actualizar Astro y dependencias oficiales
- [x] Verificar que `@astrojs/check` se actualiza a versión compatible

### 3. Limpiar configuración obsoleta
- [x] Revisar `astro.config.mjs` - eliminar `experimental.rustCompiler` si existe
- [x] Revisar `tsconfig.json` - verificar compatibilidad

### 4. Verificación
- [x] Ejecutar `npm run build` y verificar que completa sin errores
- [x] Ejecutar `npm run dev` y verificar que el sitio carga correctamente
- [x] Verificar que la ruta `http://localhost:4321/` funciona

### 5. Rollback (si falla)
- [ ] Restaurar package.json y package-lock.json desde backup
- [ ] Ejecutar `npm install`

## Notas técnicas
- **Vite 8**: Astro 7 usa Vite 8 (cambio desde Vite 5)
- **Compilador Rust**: Reemplaza al compilador Go, más rápido
- **Markdown**: Sätteri es el nuevo procesador por defecto (no afecta si no usas remark/rehype plugins)
- **Node**: Requiere ^22.12.0 || ^24.0.0

## Riesgos
- **Bajo**: Proyecto estático simple sin content collections
- **Bajo**: No usa plugins remark/rehype personalizados
- **Medio**: Dependencias externas (hotkeypad, mailtoui) podrían tener incompatibilidades

## Resultado esperado
- [x] Astro v7.0.2 funcionando
- [x] Build exitoso
- [x] Sitio web operativo en localhost:4321
