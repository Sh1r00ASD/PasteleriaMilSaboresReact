# Pastelería Mil Sabores - Sistema Completo

## 🎂 Descripción del Proyecto

Sistema web completo para una pastelería con funcionalidades de e-commerce, administración y gestión de órdenes. Desarrollado con React y Bootstrap.

## ✨ Funcionalidades Implementadas

### 🛒 Sistema de E-commerce
- **Catálogo de productos** con categorías organizadas
- **Carrito de compras** funcional con persistencia
- **Sistema de checkout** con validación completa
- **Boletas PDF** generadas automáticamente
- **Cupones de descuento** (FELICES50 - 10% descuento)
- **Descuentos especiales** para usuarios senior
- **Gestión de stock** en tiempo real

### 👤 Sistema de Usuarios
- **Registro y login** de usuarios
- **Perfil de usuario** editable
- **Recuperación de contraseña**
- **Datos temporales** para compras sin registro
- **Roles diferenciados** (cliente/admin)

### 🏪 Panel de Administración
- **Dashboard principal** con estadísticas en tiempo real
- **Gestión de productos** (CRUD completo)
- **Gestión de usuarios** (CRUD completo)
- **Gestión de órdenes** con cambio de estados
- **Gestión de categorías** (CRUD completo)
- **Reportes y estadísticas** detalladas

### 📊 Sistema de Órdenes
- **Estados de órdenes**: Pendiente → Confirmado → Preparando → Listo → Enviado → Entregado
- **Notificaciones automáticas** de cambio de estado
- **Seguimiento completo** del pedido
- **Datos de envío** persistentes
- **Métodos de pago** múltiples

### 🧪 Sistema de Testing
- **Tests unitarios** organizados y funcionales
- **Tests de componentes** con React Testing Library
- **Tests de servicios** con Jest
- **Mocks completos** para todas las dependencias
- **Cobertura de tests** amplia

## 🚀 Tecnologías Utilizadas

### Frontend
- **React 18** - Framework principal
- **React Router DOM** - Navegación
- **Bootstrap 5** - Framework CSS
- **Bootstrap Icons** - Iconografía
- **React Bootstrap** - Componentes UI

### Testing
- **Jest** - Framework de testing
- **React Testing Library** - Testing de componentes
- **Karma** - Test runner adicional

### Generación de PDFs
- **jsPDF** - Generación de PDFs
- **jspdf-autotable** - Tablas en PDF
- **html2canvas** - Captura de elementos HTML

### Utilidades
- **date-fns** - Manipulación de fechas
- **axios** - Cliente HTTP (preparado para APIs)

## 📁 Estructura del Proyecto

```
src/
├── components/
│   ├── admin/           # Componentes del panel de administración
│   │   ├── Dashboard.jsx
│   │   ├── ProductoAdmin.jsx
│   │   ├── UsuarioAdmin.jsx
│   │   ├── OrdenesAdmin.jsx
│   │   ├── CategoriaAdmin.jsx
│   │   └── Reportes.jsx
│   ├── auth/            # Componentes de autenticación
│   ├── carrito/         # Componentes del carrito de compras
│   ├── productos/       # Componentes de productos
│   └── layout/          # Componentes de layout
├── data/
│   ├── dataService.js   # Servicios de datos
│   └── regionesChile.js # Datos de regiones
├── services/
│   ├── pdfService.js    # Servicio de generación de PDFs
│   └── notificacionesService.js
├── tests/
│   ├── components/      # Tests de componentes
│   ├── services/        # Tests de servicios
│   └── utils/           # Utilidades de testing
├── utils/
│   └── initializeApp.js # Inicialización de la app
└── App.js              # Componente principal
```

## 🛠️ Instalación y Configuración

### Prerrequisitos
- Node.js (versión 16 o superior)
- npm o yarn

### Pasos de instalación

1. **Clonar el repositorio**
```bash
git clone [url-del-repositorio]
cd pasteleria-mil-sabores-main
```

2. **Instalar dependencias**
```bash
npm install
```

3. **Ejecutar en modo desarrollo**
```bash
npm start
```

4. **Ejecutar tests**
```bash
npm test
```

5. **Ejecutar tests con Karma**
```bash
npm run test:karma
```

6. **Generar build de producción**
```bash
npm run build
```

## 🎯 Funcionalidades Principales

### Para Clientes
1. **Navegación por categorías** de productos
2. **Búsqueda de productos** por nombre o descripción
3. **Agregar productos al carrito** con cantidades
4. **Aplicar cupones de descuento**
5. **Proceso de checkout** completo con validación
6. **Descarga de boletas** en formato PDF
7. **Seguimiento de pedidos** en tiempo real

### Para Administradores
1. **Dashboard con estadísticas** en tiempo real
2. **Gestión completa de productos** (crear, editar, eliminar)
3. **Gestión de usuarios** y roles
4. **Gestión de órdenes** y estados
5. **Gestión de categorías**
6. **Reportes detallados** de ventas
7. **Filtros y búsquedas** avanzadas

## 📋 Datos de Prueba

### Usuarios de Prueba
- **Admin**: admin@pasteleria.cl / 123456
- **Cliente**: maria@example.cl / 123456

### Cupones de Descuento
- **FELICES50**: 10% de descuento

### Productos de Prueba
- 14 productos en 8 categorías diferentes
- Productos con ofertas y precios especiales
- Productos personalizables y especiales (sin gluten, veganos, etc.)

## 🔧 Configuración Avanzada

### Variables de Entorno
El proyecto está preparado para usar variables de entorno. Crear un archivo `.env` en la raíz:

```env
REACT_APP_API_URL=http://localhost:3001/api
REACT_APP_APP_NAME=Pastelería Mil Sabores
```

### Personalización de Estilos
Los estilos se pueden personalizar editando:
- `src/App.css` - Estilos principales
- `src/index.css` - Estilos globales
- Variables CSS en `src/theme/colors.js`

## 🧪 Testing

### Ejecutar Tests
```bash
# Tests unitarios
npm test

# Tests con Karma
npm run test:karma

# Tests con cobertura
npm run test:coverage
```

### Estructura de Tests
- **Componentes**: Tests de renderizado, eventos y props
- **Servicios**: Tests de funciones de datos
- **Utilidades**: Tests de funciones helper

## 📦 Despliegue

### Build de Producción
```bash
npm run build
```

Los archivos se generan en la carpeta `build/` y están listos para desplegar en cualquier servidor web.

### Configuración de Servidor
El proyecto está configurado para funcionar con:
- Servidores Apache/Nginx
- CDNs
- Plataformas como Netlify, Vercel, etc.

## 🔄 Funcionalidades Futuras

### Próximas Implementaciones
- [ ] Integración con APIs reales
- [ ] Sistema de pagos online
- [ ] Notificaciones push
- [ ] App móvil
- [ ] Sistema de reviews
- [ ] Chat de soporte
- [ ] Analytics avanzados

## 🤝 Contribución

### Cómo Contribuir
1. Fork del proyecto
2. Crear rama para feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit de cambios (`git commit -m 'Agregar nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Crear Pull Request

### Estándares de Código
- Usar ESLint configurado
- Seguir convenciones de React
- Escribir tests para nuevas funcionalidades
- Documentar código complejo

## 📞 Soporte

Para soporte técnico o consultas:
- Email: soporte@mil-sabores.cl
- Documentación: [Enlace a documentación]
- Issues: [Enlace a GitHub Issues]

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

---

**Desarrollado con ❤️ para Pastelería Mil Sabores**

*Sistema completo de e-commerce para pastelería con panel de administración funcional*
