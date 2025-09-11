# Portfolio de Javier Jiménez

## 📝 Notas para el Desarrollo

### Funcionalidades Implementadas

✅ **Responsive Design completo**
- Mobile-first approach
- Breakpoints optimizados
- Layouts que se adaptan perfectamente

✅ **Dark Mode con persistencia**
- Toggle funcional en la navegación
- Estado guardado en localStorage
- Detección de preferencia del sistema

✅ **Componentes interactivos**
- Filtros de proyectos funcionales
- Formulario de contacto integrado
- Animaciones suaves con scroll

✅ **SEO y Performance**
- Meta tags completos
- Semantic HTML
- Lazy loading optimizado

### Personalización Rápida

#### Cambiar información personal:
1. **Hero.astro** - Nombre, título, descripción
2. **About.astro** - Bio personal, estadísticas, habilidades
3. **Experience.astro** - Historial laboral
4. **Contact.astro** - Email y enlaces sociales

#### Actualizar proyectos:
- Editar array de proyectos en **Projects.astro**
- Mantener estructura: `{ title, description, tech, github, demo, category, featured }`

#### Modificar publicaciones:
- Actualizar array en **Publications.astro**
- Formato: `{ title, authors, journal, year, doi, citations, impact }`

### Deployment Options

#### Vercel (Recomendado)
```bash
npm run build
# Deploy automático con git push
```

#### Netlify
```bash
npm run build
# Drag & drop de la carpeta dist/
```

#### GitHub Pages
```bash
npm run build
# Push de dist/ a rama gh-pages
```

### Scripts de Desarrollo

```bash
# Desarrollo local
npm run dev

# Build para producción
npm run build

# Preview del build
npm run preview

# Verificar tipos
npx astro check
```

### Estructura de Colores

```css
/* Principales */
--blue-600: #2563eb
--blue-700: #1d4ed8
--purple-600: #9333ea
--purple-700: #7c3aed

/* Estados */
--green-500: #10b981   /* Success */
--orange-500: #f59e0b  /* Warning */
--red-500: #ef4444     /* Error */

/* Neutrales */
--gray-50: #f9fafb     /* Background light */
--gray-900: #111827    /* Background dark */
```

### Tips de Rendimiento

1. **Imágenes**: Usa WebP cuando sea posible
2. **Iconos**: Los SVG inline son más rápidos
3. **Fonts**: Google Fonts con display=swap
4. **CSS**: Tailwind purga automáticamente

### Próximas Mejoras Sugeridas

- [ ] Blog con Astro Content Collections
- [ ] Sistema de testimonios
- [ ] Galería de certificaciones
- [ ] Integración con CMS headless
- [ ] Analytics (Google/Plausible)
- [ ] Newsletter signup
- [ ] Sitemap automático

### Solución de Problemas Comunes

#### Build fallos:
```bash
npm run astro check
npm run build -- --verbose
```

#### Estilos no se cargan:
- Verificar importaciones en Layout.astro
- Revisar sintaxis de Tailwind

#### Componentes no se muestran:
- Verificar importaciones en index.astro
- Revisar sintaxis de Astro components
