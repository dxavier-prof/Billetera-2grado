Guía Paso a Paso para Crear y Configurar tu Base de Datos en Firebase
Sigue estos sencillos pasos para crear tu proyecto gratuito en Firebase y conectarlo con la app:

1. Crear el Proyecto en Firebase
Ingresa a Firebase Console con tu cuenta de Google.

Haz clic en "Agregar proyecto" (o "Create a project").

Asigna un nombre (ej. billetera-escolar). Puedes deshabilitar Google Analytics para este proyecto y haz clic en Crear proyecto.

2. Crear la Base de Datos Firestore
En el menú lateral izquierdo, ve a Compilación (Build) -> Firestore Database.

Haz clic en Crear base de datos.

Selecciona la ubicación del servidor más cercana (ej. nam5 o us-central).

Selecciona Comenzar en modo de prueba (o modo de producción) y haz clic en Habilitar.

Ve a la pestaña Reglas (Rules) en la parte superior.

Borra el contenido existente, pega el código que te generé en el archivo firestore.rules y haz clic en Publicar.

3. Habilitar Autenticación Anónima
En el menú lateral, ve a Compilación (Build) -> Authentication.

Haz clic en Comenzar (Get Started).

En la pestaña Métodos de inicio de sesión (Sign-in method), selecciona Anónimo (Anonymous).

Activa el interruptor y haz clic en Guardar.

4. Obtener las Claves de la API (firebaseConfig)
Ve a la esquina superior izquierda y haz clic en el ícono de Engranaje (⚙️) -> Configuración del proyecto.

Desplázate hasta la sección Tus aplicaciones y haz clic en el ícono Web </>.

Registra un apodo para la app (ej. Billetera Web) y haz clic en Registrar app.

Copia el objeto const firebaseConfig = { ... }; que te aparecerá en pantalla.

Abre tu archivo index.html en el editor y reemplaza los valores de this.firebaseConfig con tus claves reales.
