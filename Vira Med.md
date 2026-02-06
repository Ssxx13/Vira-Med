# 📘 GUÍA COMPLETA: Desplegar Vademécum Digital en GitHub Pages

## 🎯 Objetivo
Publicar tu aplicación de consulta de medicamentos en GitHub Pages para que sea accesible globalmente de forma gratuita.

---

## 📋 REQUISITOS PREVIOS

Necesitarás:
1. Una cuenta de GitHub (gratis) - Si no tienes, créala en https://github.com/signup
2. El archivo `index.html` que te acabo de proporcionar

---

## 🚀 MÉTODO 1: SUBIDA DIRECTA (MÁS FÁCIL - RECOMENDADO)

### Paso 1: Crear un repositorio en GitHub

1. **Inicia sesión** en GitHub (https://github.com)

2. **Crea un nuevo repositorio:**
   - Haz clic en el botón verde **"New"** (arriba a la derecha) o el símbolo **"+"**
   - Selecciona **"New repository"**

3. **Configura el repositorio:**
   - **Repository name:** `vademecum-enfermeria-unal` (o el nombre que prefieras)
   - **Description:** "Vademécum Digital - Facultad de Enfermería UNAL"
   - **Visibilidad:** Selecciona **"Public"** (para que GitHub Pages funcione gratis)
   - ✅ **Marca** la opción: **"Add a README file"**
   - Haz clic en **"Create repository"**

### Paso 2: Subir el archivo index.html

1. **En la página principal del repositorio:**
   - Haz clic en **"Add file"** → **"Upload files"**

2. **Sube el archivo:**
   - Arrastra y suelta el archivo `index.html` 
   - O haz clic en **"choose your files"** y selecciona el archivo

3. **Confirma la subida:**
   - En el cuadro de texto inferior escribe: "Subir aplicación de vademécum"
   - Haz clic en **"Commit changes"**

### Paso 3: Activar GitHub Pages

1. **Ve a la configuración:**
   - Haz clic en **"Settings"** (pestaña en la parte superior del repositorio)

2. **Encuentra GitHub Pages:**
   - En el menú lateral izquierdo, busca **"Pages"** (en la sección "Code and automation")
   - Haz clic en **"Pages"**

3. **Configura la fuente:**
   - En **"Source"**, selecciona **"Deploy from a branch"**
   - En **"Branch"**, selecciona **"main"** (o "master")
   - En el segundo selector, deja **"/ (root)"**
   - Haz clic en **"Save"**

4. **Espera el despliegue:**
   - GitHub comenzará a construir tu sitio (toma 1-2 minutos)
   - Refresca la página después de un minuto
   - Verás un mensaje verde con tu URL: 
     ```
     Your site is live at https://TU-USUARIO.github.io/vademecum-enfermeria-unal/
     ```

### Paso 4: ¡Listo! Prueba tu aplicación

Abre la URL en tu navegador y verás tu Vademécum Digital funcionando.

---

## 🔄 MÉTODO 2: USANDO GIT (Para actualizaciones frecuentes)

Si planeas hacer muchas actualizaciones, es mejor usar Git desde tu computadora:

### Instalación inicial:

1. **Instala Git:**
   - Windows: https://git-scm.com/download/win
   - Mac: Ya viene instalado (o usa `brew install git`)
   - Linux: `sudo apt-get install git`

2. **Configura Git (solo una vez):**
   ```bash
   git config --global user.name "Tu Nombre"
   git config --global user.email "tu-email@ejemplo.com"
   ```

### Subir tu proyecto:

1. **Abre la terminal/CMD en la carpeta donde tienes index.html**

2. **Ejecuta estos comandos uno por uno:**
   ```bash
   # Inicializar repositorio Git
   git init
   
   # Agregar el archivo
   git add index.html
   
   # Hacer el primer commit
   git commit -m "Primera versión del vademécum"
   
   # Conectar con tu repositorio de GitHub (reemplaza TU-USUARIO y TU-REPO)
   git remote add origin https://github.com/TU-USUARIO/vademecum-enfermeria-unal.git
   
   # Subir los cambios
   git branch -M main
   git push -u origin main
   ```

3. **Sigue el Paso 3 del Método 1** para activar GitHub Pages

### Para actualizar en el futuro:

```bash
# Después de hacer cambios en index.html
git add index.html
git commit -m "Descripción del cambio"
git push
```

¡Los cambios se reflejarán automáticamente en 1-2 minutos!

---

## ✏️ CÓMO ACTUALIZAR TU APLICACIÓN

### Opción A: Desde GitHub (Web - MÁS FÁCIL)

1. Ve a tu repositorio en GitHub
2. Haz clic en el archivo `index.html`
3. Haz clic en el ícono del lápiz (✏️) "Edit this file"
4. Haz tus cambios
5. Abajo, escribe una descripción del cambio
6. Haz clic en **"Commit changes"**
7. Los cambios se publicarán automáticamente en 1-2 minutos

### Opción B: Reemplazar archivo completo

1. Ve a tu repositorio
2. Haz clic en `index.html` → Los tres puntos (...) → **"Delete file"**
3. Confirma la eliminación
4. Sube el nuevo archivo usando **"Add file" → "Upload files"**

### Opción C: Usando Git (desde tu computadora)

```bash
# Hacer cambios en index.html con tu editor preferido
# Luego ejecutar:
git add index.html
git commit -m "Actualización: agregados 10 nuevos medicamentos"
git push
```

---

## 🎨 PERSONALIZACIÓN RECOMENDADA

### Cambiar el nombre en el título:
Busca en `index.html` la línea:
```html
<title>Vademécum Digital - Enfermería UNAL</title>
```

### Cambiar la contraseña de administrador:
Busca en el código:
```javascript
if (password === 'admin123') {
```
Cambia `'admin123'` por tu contraseña deseada.

---

## 📱 COMPARTIR TU APLICACIÓN

Una vez publicada, puedes compartir el link:
```
https://TU-USUARIO.github.io/vademecum-enfermeria-unal/
```

Puedes crear un código QR para facilitar el acceso:
- Ve a: https://www.qr-code-generator.com/
- Pega tu URL
- Descarga el código QR
- Imprime y coloca en lugares estratégicos de la facultad

---

## 🔐 SEGURIDAD Y BUENAS PRÁCTICAS

1. **Cambiar la contraseña de administrador** (ver sección de Personalización)
2. **Hacer backups regulares:** Descarga tu repositorio cada cierto tiempo
3. **No compartir la contraseña de admin públicamente**
4. **Revisar cambios antes de publicar**

---

## 🆘 SOLUCIÓN DE PROBLEMAS

### Problema: "404 - Page not found"
**Solución:** 
- Verifica que GitHub Pages esté activado en Settings → Pages
- Asegúrate de que el archivo se llame exactamente `index.html` (minúsculas)
- Espera 2-5 minutos después de activar GitHub Pages

### Problema: Los cambios no se reflejan
**Solución:**
- Espera 1-2 minutos después de hacer push
- Limpia el caché del navegador (Ctrl + F5 o Cmd + Shift + R)
- Verifica en el repositorio que los cambios sí se subieron

### Problema: La aplicación no funciona correctamente
**Solución:**
- Abre la consola del navegador (F12)
- Busca errores en la pestaña "Console"
- Verifica que todas las librerías se carguen correctamente

---

## 📊 MONITOREO Y ESTADÍSTICAS

### Ver estadísticas de visitas:

1. **Opción gratuita - Google Analytics:**
   - Crea una cuenta en https://analytics.google.com
   - Agrega el código de tracking en el `<head>` de tu index.html
   
2. **Ver tráfico básico de GitHub:**
   - Ve a tu repositorio → **Insights** → **Traffic**
   - Muestra visitas de las últimas 2 semanas

---

## 🎓 PRÓXIMOS PASOS SUGERIDOS

Una vez que tu aplicación esté funcionando:

1. **Agregar todos los medicamentos** usando el panel de administrador
2. **Hacer un backup** descargando el repositorio completo
3. **Compartir el link** con estudiantes y profesores
4. **Crear material de soporte:** Guía rápida de uso, videos tutoriales
5. **Considerar un dominio personalizado** (opcional):
   - Ejemplo: `vademecum-enfermeria.unal.edu.co`
   - Requiere coordinación con el área de IT de la UNAL

---

## 📞 AYUDA ADICIONAL

- **Documentación oficial de GitHub Pages:** https://docs.github.com/es/pages
- **Soporte de GitHub:** https://support.github.com/
- **Comunidad de GitHub:** https://github.community/

---

## ✅ CHECKLIST FINAL

Antes de compartir públicamente, verifica:

- [ ] La aplicación carga correctamente en tu navegador
- [ ] Puedes buscar y filtrar medicamentos
- [ ] El panel de administrador funciona con tu contraseña
- [ ] Puedes agregar, editar y eliminar medicamentos
- [ ] Los datos persisten después de recargar la página
- [ ] La aplicación es responsive (funciona en móvil)
- [ ] Has cambiado la contraseña por defecto
- [ ] Has agregado al menos los primeros medicamentos
- [ ] El título y descripción son correctos

---

¡Éxito con tu Vademécum Digital! 🎉

**Fecha de creación:** Febrero 2026
**Versión:** 1.0