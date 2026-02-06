# 💊 Vademécum Digital - Enfermería UNAL

Sistema de consulta de medicamentos desarrollado para la Facultad de Enfermería de la Universidad Nacional de Colombia.

![Version](https://img.shields.io/badge/version-1.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

## 📋 Descripción

Aplicación web para consulta de información farmacológica completa, diseñada específicamente para estudiantes y profesionales de enfermería. Incluye información detallada sobre posología, mecanismos de acción, interacciones, y protocolos de administración.

## ✨ Características

### Para Usuarios Generales (Consulta)
- 🔍 **Búsqueda rápida** por nombre o familia farmacológica
- 🎯 **Filtros avanzados** por familia farmacológica y presentación
- 📊 **Ordenamiento alfabético** (A-Z / Z-A)
- 📱 **Responsive** - funciona en móviles, tablets y computadoras
- 💾 **Datos persistentes** - la información se mantiene entre sesiones

### Para Administradores
- ➕ **Agregar nuevos medicamentos**
- ✏️ **Editar medicamentos existentes**
- 🗑️ **Eliminar registros**
- 🔒 **Acceso protegido por contraseña**

## 📊 Información de cada Medicamento

Cada registro incluye:
- ✅ Nombre del medicamento
- ✅ Presentación
- ✅ Posología
- ✅ Mecanismo de acción
- ✅ Reacciones adversas
- ✅ Rango terapéutico
- ✅ Perfusión y velocidad
- ✅ Reconstitución y dilución
- ✅ Estabilidad
- ✅ pH, Osmolaridad, Densidad
- ✅ Clasificación vesicante/irritante
- ✅ Observaciones especiales
- ✅ Familia farmacológica

## 🚀 Demo en Vivo

**[Ver aplicación en vivo](https://TU-USUARIO.github.io/vademecum-enfermeria-unal/)**

*(Reemplaza con tu URL de GitHub Pages una vez desplegado)*

## 🔐 Acceso de Administrador

Para acceder al panel de administración:
- Usuario: Administrador
- Contraseña: `admin123` *(Cambiar después del primer uso)*

## 🛠️ Tecnologías Utilizadas

- **React 18** - Framework JavaScript
- **Tailwind CSS** - Estilos y diseño responsive
- **Lucide Icons** - Iconografía
- **LocalStorage API** - Persistencia de datos

## 📥 Instalación Local

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/TU-USUARIO/vademecum-enfermeria-unal.git
   cd vademecum-enfermeria-unal
   ```

2. **Abrir en el navegador:**
   - Simplemente abre `index.html` con tu navegador favorito
   - No requiere instalación de dependencias

## 🔄 Actualizar la Aplicación

### Método 1: Desde GitHub (Web)
1. Ve al repositorio en GitHub
2. Haz clic en `index.html` → Editar (ícono del lápiz)
3. Realiza los cambios
4. Guarda con "Commit changes"

### Método 2: Desde tu computadora
```bash
# Hacer cambios en index.html
git add index.html
git commit -m "Descripción del cambio"
git push
```

Los cambios se reflejarán automáticamente en 1-2 minutos.

## 📱 Uso

### Para Estudiantes/Consulta:
1. Usa la barra de búsqueda para encontrar medicamentos
2. Aplica filtros por familia farmacológica o presentación
3. Haz clic en "Ver más" para información detallada
4. Los datos se mantienen al recargar la página

### Para Administradores:
1. Haz clic en "Acceso Admin"
2. Ingresa la contraseña
3. Usa "Nuevo Medicamento" para agregar registros
4. Edita o elimina medicamentos con los botones correspondientes

## 🔐 Seguridad

### Cambiar la Contraseña de Administrador

Busca en `index.html` la línea:
```javascript
if (password === 'admin123') {
```

Cámbiala por:
```javascript
if (password === 'TU_NUEVA_CONTRASEÑA') {
```

## 🤝 Contribuir

Este es un proyecto académico de la UNAL. Para contribuir:

1. Haz fork del repositorio
2. Crea una rama para tu característica (`git checkout -b feature/nueva-caracteristica`)
3. Commit tus cambios (`git commit -m 'Agregar nueva característica'`)
4. Push a la rama (`git push origin feature/nueva-caracteristica`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## 👥 Autores

**Facultad de Enfermería - Universidad Nacional de Colombia**

## 🙏 Agradecimientos

- Estudiantes de Enfermería UNAL
- Profesores colaboradores
- Comunidad de desarrollo open source

## 📞 Contacto

Para preguntas o sugerencias sobre el proyecto:
- 📧 Email: enfermeria@unal.edu.co
- 🌐 Web: https://enfermeria.unal.edu.co

## 📈 Roadmap

- [x] Versión 1.0 - Funcionalidad básica
- [ ] Versión 1.1 - Exportar datos a PDF
- [ ] Versión 1.2 - Sistema de favoritos
- [ ] Versión 1.3 - Modo oscuro
- [ ] Versión 2.0 - Integración con calculadoras de dosis

## 🐛 Reportar Problemas

Si encuentras un bug o tienes una sugerencia, por favor:
1. Abre un [Issue](https://github.com/TU-USUARIO/vademecum-enfermeria-unal/issues)
2. Describe el problema detalladamente
3. Incluye capturas de pantalla si es posible

---

**Desarrollado con ❤️ para la comunidad de Enfermería UNAL**

*Última actualización: Febrero 2026*