# TicketPro+

TicketPro+ es una plataforma para gestionar solicitudes y tickets de manera eficiente. Nuestra aplicación está diseñada para facilitar la comunicación entre usuarios y administradores, ofreciendo una solución integral para el soporte técnico.

## Estructura del Proyecto

```plaintext
client/                                      # Código del lado del cliente
├── assets/                                  # Archivos estáticos utilizados en la aplicación
│   ├── css/                                 # Hojas de estilo CSS
│   │   ├── tailwind.css                     # Archivo CSS generado por Tailwind
│   │   ├── styles.css                       # Hoja de estilos generales de la aplicación
│   ├── images/                              # Imágenes usadas en la aplicación
│   │   ├── logoticket.png                   # Imagen del logo principal
│   │   └── logoticket2.png                  # Imagen del logo secundario
│   └── js/                                  # Archivos JavaScript para la lógica del cliente
│       ├── actualizarCamposPrograma.js      # Script que actualiza campos de tipología y modalidad
│       ├── cargarProgramas.js               # Script que carga programas desde el servidor
│       ├── cargarTipologiasYSubtipologias.js# Script que carga tipologías y subtipologías
│       ├── handleError.js                   # Script para manejar errores
│       ├── inicializarFunciones.js          # Inicialización de funciones de la app
│       ├── jquery.min.js                    # Biblioteca jQuery
│       ├── menu.js                          # Script para el menú
│       ├── mistickets.js                    # Script para gestionar los tickets del usuario
│       ├── sidebar.js                       # Script para la barra lateral
│       ├── sweetalert2.js                   # Biblioteca SweetAlert2 para mostrar alertas
│       └── tickets.js                       # Script para cargar estados de tickets
├── partials/                                # Fragmentos HTML reutilizables
│   ├── header.html                          # Encabezado común
│   ├── footer.html                          # Pie de página común
│   ├── sidebar.html                         # Barra lateral común
├── pages/                                   # Páginas HTML principales
│   ├── home.html                            # Página de inicio
│   ├── tickets.html                         # Página de tickets
│   ├── perfil.html                          # Página de perfil del usuario
│   ├── contacto.html                        # Página de contacto
├── auth/                                    # Páginas HTML relacionadas con la autenticación
│   ├── login.html                           # Página de inicio de sesión
│   ├── register.html                        # Página de registro de usuarios
│   ├── password_recovery.html               # Página de recuperación de contraseña
├── index.html                               # Punto de entrada principal del cliente
├── tailwind.config.js                       # Configuración de Tailwind CSS
├── postcss.config.js                        # Configuración de PostCSS
├── package.json                             # Dependencias del proyecto
├── [README.md](http://_vscodecontentref_/1)                                # Descripción del cliente

server/                                      # Código del lado del servidor
├── config/                                  # Configuraciones del servidor
│   └── config.php                           # Configuración de conexión a la base de datos
├── controllers/                             # Controladores para manejar la lógica de negocio
│   ├── AuthController.php                   # Controlador para autenticación
│   ├── TicketController.php                 # Controlador para gestión de tickets
│   └── UserController.php                   # Controlador para gestión de usuarios
├── models/                                  # Modelos para interactuar con la base de datos
│   ├── Role.php                             # Modelo para roles
│   ├── Permission.php                       # Modelo para permisos
│   ├── Ticket.php                           # Modelo para tickets
│   └── User.php                             # Modelo para usuarios
├── routes/                                  # Rutas de la aplicación
│   ├── api.php                              # Rutas para la API
│   └── web.php                              # Rutas para la web
├── views/                                   # Vistas del servidor
│   ├── auth/                                # Vistas de autenticación
│   ├── dashboard/                           # Vistas del dashboard
│   ├── errors/                              # Vistas de errores
│   ├── layouts/                             # Layouts comunes
│   └── tickets/                             # Vistas de tickets
├── database/                                # Base de datos y scripts relacionados
│   ├── migrations/                          # Migraciones de la base de datos
│   ├── seeds/                               # Datos de prueba
│   └── bdticketpro.sql                      # Esquema de la base de datos
├── logs/                                    # Archivos de registro para errores y eventos
│   └── app.log                              # Registro de errores y eventos de la aplicación
├── tests/                                   # Pruebas del servidor
│   ├── functional/                          # Pruebas funcionales
│   └── unit/                                # Pruebas unitarias
├── .gitignore                               # Archivo para ignorar archivos y carpetas en el control de versiones
├── [README.md](http://_vscodecontentref_/2)                                # Descripción del servidor
├── composer.json                            # Dependencias de PHP
└── public/                                  # Carpeta pública accesible desde el navegador
    ├── [index.php](http://_vscodecontentref_/3)                            # Punto de entrada principal del servidor
    ├── .htaccess                            # Configuraciones de Apache (si es necesario)
    └── assets/                              # Archivos estáticos accesibles públicamente
        ├── css/                             # Hojas de estilo CSS
        ├── images/                          # Imágenes usadas en la aplicación
        └── js/                              # Archivos JavaScript para la lógica del cliente