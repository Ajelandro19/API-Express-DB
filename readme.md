# Dependencias
<ul>
  <dt>JEST</dt><dd>Para pruebas unitarias. <code>npm install --save-dev jest</code></dd>
  <dt>Eslint</dt><dd>Para corrección de estilo de código. <code>npm install eslint --save-dev</code></dd>
  <dt>Express</dt><dd>Para crear un servidor básico. <code>npm install express --save-dev</code></dd>
  <dt>Prisma</dt><dd>Para conectarse a Postgresql. <code>npm install prisma --save-dev</code></dd>
</ul>

## Configurar eslint
> npm init @eslint/config

## Inicializar Prisma
>npx prisma init
Información sobre npx en: https://docs.npmjs.com/cli/v7/commands/npx
## Versionar db con Prisma (Migrations)
>npx prisma migrate dev --name init


# Endpoints

| Endpoint | Request | Response | Método |
|---|---|---|---|
| `localhost:3000/explorers` | `...` | Deberás obtener la lista de explorers| GET|
| `localhost:3000/explorers/:id` | `localhost:3000/v1/explorers/2` | Deberás obtener el explorer del ID proporcionado| GET |
| `localhost:3000/explorers` | `{name: , username: , mission: }` | Crearás un nuevo explorer| POST |
| `localhost:3000/explorers/:id` | `{mission: }` | Actualizarás la misión del explorer con el ID dado| PUT |
| `localhost:3000/explorers/:id` | `...` | Eliminarás el explorer con el ID dado| DELETE |
| `localhost:3000/students` | `...` | Deberás obtener la lista de students| GET |
| `localhost:3000/students/:id` | `localhost:3000/v1/explorers/2` | Deberás obtener el student del ID proporcionado| GET |
| `localhost:3000/students` | `{name: , lang: , missionCommander: }` | Crearás un nuevo student | POST |
| `localhost:3000/students/:id` | `{missionCommander: }` | Actualizarás el MC del student con el ID dado| PUT |
| `localhost:3000/students/:id` | `...` | Eliminarás el explorer con el ID dado | DELETE |



# Preparar el servidor con CORS

  1. Instalar la dependencia CORS: `npm install cors --save` 