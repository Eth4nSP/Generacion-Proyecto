# Base de Proyecto Node.js con CI/CD

Este repositorio contiene la plantilla base y configuración de infraestructura para el desarrollo de software bajo estándares profesionales.

## Tecnologías Integradas

- **Entorno:** Node.js, TypeScript.
- **Calidad de Código:** ESLint 8 (Linter), Prettier (Formateador).
- **Pruebas:** Jest, ts-jest (TDD).
- **Automatización Local:** Husky, lint-staged (Git Hooks).
- **Integración Continua:** GitHub Actions (`ci.yml`).

## Comandos Disponibles

- `npm run lint`: Evalúa el código buscando errores de sintaxis y malas prácticas.
- `npm run format`: Aplica el formato automático de Prettier a todo el proyecto.
- `npm run format:check`: Verifica si los archivos cumplen con el formato (usado en CI).
- `npm test`: Ejecuta la suite de pruebas unitarias.
- `npm run build`: Compila el proyecto TypeScript.

## Flujo de Trabajo

El proyecto está protegido por **Husky**:
1. Al hacer `git commit`, se formatea automáticamente el código preparado.
2. Al hacer `git push`, se ejecutan todas las pruebas unitarias para evitar romper la rama remota.
