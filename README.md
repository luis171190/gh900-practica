# GH-900 Práctica

Repo de práctica para preparar la certificación **GitHub Foundations (GH-900)**.
Cada archivo de acá existe para tocar a mano un tema del examen.

> [!NOTE]
> Esto es un bloque de alerta de GitHub (Markdown extendido). Hay cinco tipos:
> `NOTE`, `TIP`, `IMPORTANT`, `WARNING` y `CAUTION`.

## Mapa: archivo → tema del examen

| Archivo | Tema del examen | Peso |
|---|---|---|
| `README.md` | Markdown para comunicar | 25-30% (básico) |
| `LICENSE`, `CONTRIBUTING.md`, `SECURITY.md` | Archivos clave de un repo | 10-15% (repos) |
| `.github/CODEOWNERS` | Archivos clave + revisión de PRs | 10-15% (repos) |
| `.github/ISSUE_TEMPLATE/`, `.github/pull_request_template.md` | Plantillas de colaboración | 10-15% (colaboración) |
| `.github/workflows/hola.yml` | GitHub Actions | 10-15% (desarrollo moderno) |
| `.devcontainer/devcontainer.json` | Codespaces y dev containers | 10-15% (desarrollo moderno) |
| `GUIA.md` | Lo que se hace en la web (Projects, protección de ramas, Wiki, Pages) | varios |

## Markdown que entra en el examen

Lista de tareas (en un issue se ve como checkboxes y cuenta el progreso):

- [x] Crear el repo local
- [ ] Subirlo a GitHub
- [ ] Hacer el primer PR enlazado a un issue

Código con resaltado:

```bash
git switch -c feat/mi-primer-cambio
```

Menciones y referencias (funcionan en issues y PRs, no en este README):

- `@usuario` notifica a una persona.
- `#12` enlaza al issue o PR número 12.
- `Closes #12` en la descripción de un PR cierra el issue 12 cuando se mergea.

Link a la guía: [GUIA.md](GUIA.md)
