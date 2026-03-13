🛹 SkateConnect
=============
SkateConnect es una aplicación web para la gestión y reserva de espacios de skate.
Permite a los usuarios reservar pistas o espacios disponibles, cancelar reservas y consultar su historial, mientras que los administradores pueden gestionar el sistema y visualizar reportes.

El objetivo del proyecto es ofrecer una plataforma simple para organizar reservas de espacios deportivos, evitando conflictos de horarios y permitiendo una mejor administración.

🚀 Características
-------------
- 🔐 Autenticación de usuarios
  - Registro
  - Inicio de sesión
- 👥 Sistema de roles
  - ADMIN → control total del sistema
  - DIRECTORIO → acceso a reportes y gestión limitada
  - USUARIO → puede reservar, cancelar y ver su historial
- 🛹 Gestión de reservas
  - Crear reservas
  - Cancelar reservas
  - Seleccionar espacios disponibles
  - Definir número de participantes
- 🧾 Facturación
  - Generación de facturas en PDF
  - Historial de facturación por usuario
- 📊 Panel de administración
  - Visualización de reservas
  - Reportes del sistema

🏗️ Tecnologías utilizadas
-------------
Backend
----
- Python
- Flask
- MySQL

Frontend
----
- HTML5
- CSS3
- JavaScript

Librerías
----
- ReportLab (generación de PDF) 

⚙️ Instalación
-------------
Clonar el repositorio
----
```javascript
$ git clone https://github.com/ElHackerDaniel/SkateConnect.git
```

```javascript
$ cd skateconnect
```

Crear entorno virtual (opcional)
----
```javascript
$ python -m venv venv
```

Activarlo:

Windows

`$ venv\Scripts\activate`

Linux / Mac

`$ source venv/bin/activate`

Instalar dependencias
----
```javascript
$ pip install flask mysql-connector-python reportlab
```

Configurar la base de datos
----
Editar el archivo:

`config/db_config.py`

Con tus credenciales de MySQL.

Ejemplo:

```javascript
host = "localhost"
user = "root"
password = ""
database = "skateconnect"
```
Ejecutar el proyecto
----
`python app.py`

Abrir en el navegador:

`http://localhost:5000`

En esta parte podrias ir a ver las instructions.txt para el link https

👤 Roles del sistema
-------------
| Rol      | Permisos |
| :---------: | :-----:|
| Admin  | Gestiona usuarios, reservas y reportes |
| Directorio     |  Visualiza reportes |
| Usuario      | Realiza reservas y consulta historial |

📄 Generación de facturas
-------------
Cada reserva genera una factura en PDF que incluye:
- ID de la reserva
- Usuario
- Espacio reservado
- Fecha
- Hora
- Participantes

Las facturas se guardan en:

`/facturas`

📌 Posibles mejoras futuras
-------------
- Pagos en línea
- Notificaciones por correo
- Calendario visual de reservas
- Panel de estadísticas
- API REST

👨‍💻 Autor
----
Proyecto desarrollado como parte de aprendizaje en desarrollo web con Python y bases de datos.

Att: ElHackerDaniel

Inicio
----
<img width="1831" height="863" alt="inicio" src="https://github.com/user-attachments/assets/e2e25618-1285-493f-ba97-7796d35df531" />

Panel de usuario
----
<img width="1832" height="863" alt="panel usuario" src="https://github.com/user-attachments/assets/6f8eade3-d295-4bc9-bbe4-a7040df0d4ff" />

Historia de usuario
----
<img width="1827" height="862" alt="historial" src="https://github.com/user-attachments/assets/0dbb9277-f0a0-489e-9c84-be65390aaf7d" />

Panel admin
----
<img width="1832" height="861" alt="Paneladmin" src="https://github.com/user-attachments/assets/8d250112-42c9-43b6-8b68-4b9bbe9f8419" />

Panel director
----
<img width="1822" height="862" alt="Panel director" src="https://github.com/user-attachments/assets/695fdad2-f623-40cc-977a-5a743f05ee7c" />

Informe director
----
![WhatsApp Image 2026-03-13 at 12 25 37 AM](https://github.com/user-attachments/assets/98eeac79-dc23-44a4-84d9-8c0f71e4c7eb)


