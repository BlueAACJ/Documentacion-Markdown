### Configuración inicial (solo la primera vez)

Antes de iniciar, asegúrate de:
1. Tener PostgreSQL configurado y la base de datos creada.
2. Configurar la cadena de conexión a la base de datos en tu aplicación Flask o en el archivo config.py

```bash
# Ejecuta este comando para inicializar las migraciones:
flask db init

# Actualizar modelos y aplicar cambios
# Genera un archivo de migración:
flask db migrate -m "Descripción de los cambios"

# Aplica los cambios en la base de datos:
flask db upgrade

# Deshacer cambios en la base de datos

# Deshacer la última migración:
flask db downgrade

# Deshacer a una migracion especifica 
flask db downgrade <revision_id>

# Ver historial de migraciones
flask db history

# Eliminar todo y empezar de 0 
DROP DATABASE <your_database_name>;

Remove-Item -Recurse -Force migrations
