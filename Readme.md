# App Full Stack

## Database

Crea la tabla:

```sql
DROP TABLE IF EXISTS tareas;

CREATE TABLE tareas (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    persona VARCHAR NOT NULL,
    descripcion VARCHAR NOT NULL
);
```

Inserta un par de ejemplos:

```
INSERT INTO tareas (id, persona, descripcion)
VALUES
    ('550e8400-e29b-41d4-a716-446655440000', 'Manuel', 'Aprender SQLAlchemy'),
    ('550e8400-e29b-41d4-a716-446655440001', 'Lucía', 'Crear una API con FastAPI');
```

Busca la url de conexión a tu base de datos para usarla más adelante (DATABASE_URL).

## Backend-API

1. Crea el archivo .env y añade la url de conexión a la base de datos.

```
DATABASE_URL=postgresql://neondb...
```

2. Configura la carpeta source y dale al play

## Frontend-Web

Arranca el archivo `index.html` en tu navegador.

Configura la variable `API_URL` con la url de tu backend (por ejemplo, `http://localhost:8000`).
