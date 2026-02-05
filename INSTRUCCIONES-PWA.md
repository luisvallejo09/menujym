# 📱 J&M FAST FOOD - INSTALACIÓN PWA

## ✅ CAMBIOS REALIZADOS:

### 1. **BARRA DE CATEGORÍAS FIJA** 🔧
- ✅ La barra de categorías ahora se mantiene fija al hacer scroll
- ✅ Se posiciona justo debajo del header (60px desde arriba)
- ✅ Tiene mejor contraste y efecto blur
- ✅ Se eliminó el banner de promoción que interfería

### 2. **BOTÓN INSTALAR APP** 📲
- ✅ Nuevo botón flotante en la esquina superior derecha
- ✅ Solo aparece en navegadores compatibles (Chrome, Edge, Samsung Internet)
- ✅ Se oculta automáticamente si ya está instalada
- ✅ Animación de pulso para llamar la atención

---

## 📦 ARCHIVOS INCLUIDOS:

1. **index.html** - Página principal actualizada
2. **manifest.json** - Configuración de la PWA
3. **sw.js** - Service Worker (para funcionamiento offline)

---

## 🚀 CÓMO INSTALAR EN TU SERVIDOR:

### Opción A: Servidor Web Tradicional
```bash
1. Sube los 3 archivos a la raíz de tu servidor
2. Asegúrate que estén en:
   - tudominio.com/index.html
   - tudominio.com/manifest.json
   - tudominio.com/sw.js

3. ¡Listo! La app ya es instalable
```

### Opción B: GitHub Pages (GRATIS)
```bash
1. Crea un repositorio en GitHub
2. Sube los 3 archivos
3. Activa GitHub Pages en Settings
4. Accede a: usuario.github.io/nombre-repo
```

### Opción C: Netlify (GRATIS)
```bash
1. Arrastra los archivos a netlify.com/drop
2. Obtén tu URL en segundos
3. ¡Ya está funcionando!
```

---

## 📱 CÓMO INSTALAR LA APP (USUARIOS):

### En Android (Chrome/Edge):
1. Abre la página en Chrome o Edge
2. Presiona el botón **"INSTALAR APP"** 📱
3. O usa el menú: ⋮ > "Instalar aplicación"
4. Confirma la instalación
5. ¡La app aparecerá en tu pantalla de inicio!

### En iPhone/iPad (Safari):
1. Abre la página en Safari
2. Presiona el botón de **Compartir** (cuadro con flecha)
3. Selecciona **"Añadir a pantalla de inicio"**
4. Cambia el nombre si quieres
5. Presiona **"Añadir"**
6. ¡Listo! Tendrás el ícono en tu home screen

### En Computadora (Chrome/Edge):
1. Abre la página
2. Presiona el botón **"INSTALAR APP"** 📱
3. O usa el ícono de instalación en la barra de direcciones
4. ¡La app se abre en su propia ventana!

---

## ⚙️ CARACTERÍSTICAS PWA:

✅ **Funciona Offline** - Cache básico de páginas
✅ **Instalable** - Como app nativa
✅ **Pantalla Completa** - Sin barra del navegador
✅ **Ícono en Home** - Acceso rápido
✅ **Notificaciones** - (Puedes agregar después)
✅ **Rápida** - Carga optimizada

---

## 🎨 PERSONALIZACIÓN FUTURA:

### Para agregar ícono personalizado:
1. Crea una imagen cuadrada de 512x512px
2. Súbela a tu servidor
3. Actualiza las URLs en **manifest.json**:
```json
"icons": [
  {
    "src": "/ruta/a/tu/icono-512.png",
    "sizes": "512x512",
    "type": "image/png"
  }
]
```

### Para cambiar colores:
En **manifest.json**:
```json
"background_color": "#TU_COLOR",
"theme_color": "#TU_COLOR"
```

---

## 🔍 VERIFICAR QUE FUNCIONA:

### Chrome DevTools:
1. Abre DevTools (F12)
2. Ve a la pestaña **"Application"**
3. Revisa:
   - ✅ Manifest
   - ✅ Service Workers
   - ✅ Cache Storage

### Lighthouse (Auditoría PWA):
1. Abre DevTools (F12)
2. Ve a **"Lighthouse"**
3. Selecciona **"Progressive Web App"**
4. Click en **"Generate report"**
5. Deberías obtener 90+ puntos

---

## ⚠️ REQUISITOS IMPORTANTES:

### 1. HTTPS es OBLIGATORIO
- Las PWA **solo funcionan con HTTPS**
- Excepciones: localhost (desarrollo)
- Usa certificado SSL gratuito: Let's Encrypt

### 2. Servidor configurado correctamente
- Los archivos deben estar accesibles
- MIME types correctos:
  - manifest.json → `application/json`
  - sw.js → `application/javascript`

---

## 🐛 PROBLEMAS COMUNES:

### "El botón no aparece"
- ✅ Verifica que estés usando HTTPS
- ✅ Usa Chrome, Edge o Samsung Internet
- ✅ Limpia cache y recarga (Ctrl+Shift+R)
- ✅ Abre en modo incógnito para probar

### "Service Worker no se registra"
- ✅ Verifica la consola de errores (F12)
- ✅ Asegúrate que sw.js esté en la raíz
- ✅ Revisa que el MIME type sea correcto

### "La app no funciona offline"
- ✅ Espera unos segundos después de la primera visita
- ✅ El Service Worker necesita tiempo para cachear
- ✅ Actualiza el sw.js si cambias archivos

---

## 📊 PRÓXIMOS PASOS:

1. **Notificaciones Push** - Avisar de promociones
2. **Geolocalización** - Delivery inteligente
3. **Modo Oscuro** - Ahorro de batería
4. **Sincronización Background** - Pedidos offline
5. **Share API** - Compartir productos

---

## 🆘 SOPORTE:

Si tienes problemas:
1. Verifica la consola del navegador (F12)
2. Usa Lighthouse para diagnóstico
3. Revisa que todos los archivos estén subidos
4. Confirma que HTTPS esté activo

---

## 📈 ESTADÍSTICAS:

Para ver cuántas personas instalan:
- Google Analytics
- Firebase Analytics
- Eventos personalizados en el código

---

¡Disfruta tu nueva Progressive Web App! 🎉🍔
