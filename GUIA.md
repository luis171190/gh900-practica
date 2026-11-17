# Guía de ejercicios GH-900

Los archivos del repo ya están hechos (fase 1: "te lo muestro resuelto").
Esta guía es la fase 2 y 3: lo que **hacés vos** en la web de GitHub.
Marcá cada casilla cuando lo termines.

> [!IMPORTANT]
> El repo tiene que ser **público**. Con la cuenta gratis, la protección de ramas,
> la Wiki y GitHub Pages solo funcionan en repos públicos. No tiene datos personales.

## 0. Subirlo (5 min)

Desde esta carpeta:

```bash
gh repo create gh900-practica --public --source . --push
```

- [ ] El repo aparece en github.com/luis171190/gh900-practica
- [ ] En la pestaña **Actions** corrió "Hola Actions" en verde

## 1. Configuración del repo (Settings → General)

- [ ] Activá **Discussions** (la plantilla de issues apunta ahí)
- [ ] Verificá que **Wiki** e **Issues** estén activos
- [ ] Mirá el link a `CONTRIBUTING.md` que aparece al abrir un issue

## 2. Issues con plantilla

- [ ] **New issue** → elegí "Reporte de error". Fijate que es un formulario, no texto libre
- [ ] Probá el botón de issue en blanco: no aparece (lo apagó `config.yml`)
- [ ] Agregale una etiqueta (label) y asignátelo (assignee)

## 3. El flujo completo: rama → PR → merge (GitHub Flow)

```bash
git switch -c docs/primer-cambio
# editá el README, cualquier cosa
git commit -am "docs: update readme"
git push -u origin docs/primer-cambio
```

- [ ] Abrí el PR: la descripción ya viene con la plantilla
- [ ] Escribí `Closes #1` (el número de tu issue)
- [ ] Mirá cómo corre el check de Actions dentro del PR
- [ ] Mergeá y verificá que el issue #1 se cerró solo

## 4. Proteger la rama main (Settings → Rules → Rulesets)

- [ ] Creá un ruleset para `main`: exigir PR antes de mergear y exigir el check `saludo`
- [ ] Intentá `git push` directo a main: tiene que rechazarlo

> [!TIP]
> "Require review from Code Owners" no lo actives: sos el único dueño y GitHub no te deja
> aprobar tu propio PR. En el examen sí preguntan para qué sirve.

## 5. Projects (5-10% del examen)

- [ ] Creá un Project desde tu perfil y vinculalo al repo
- [ ] Probá las tres vistas: **Table**, **Board** y **Roadmap**
- [ ] Creá un **milestone** ("Semana 1") y asignale el issue
- [ ] Creá una **saved reply** (Settings de tu cuenta → Saved replies) y usala en un comentario

## 6. Documentar y compartir

- [ ] **Wiki**: creá una página "Notas"
- [ ] **Pages**: Settings → Pages → Deploy from branch `main` / root. Abrí la URL que te da
- [ ] **Gist**: creá uno en gist.github.com con un comando que uses seguido

## 7. Desarrollo moderno

- [ ] **github.dev**: en el repo apretá la tecla `.` (punto). Es un editor en el navegador, gratis, **sin terminal**
- [ ] **Codespaces**: Code → Codespaces → Create. Es una máquina virtual **con terminal**; usa el `.devcontainer/devcontainer.json`. Consume cuota gratis mensual: **apagalo al terminar**
- [ ] **Actions**: corré el workflow a mano (Actions → Hola Actions → Run workflow)
- [ ] **Copilot**: leé la página de planes (Free, Pro, Business, Enterprise) y anotá qué agrega cada uno

## 8. Seguridad y administración

- [ ] Revisá que tu cuenta tenga **2FA** o **passkey** (Settings → Password and authentication)
- [ ] Settings → Collaborators: mirá los roles **Read, Triage, Write, Maintain, Admin** y qué puede cada uno
- [ ] Security → activá **Private vulnerability reporting** (el `SECURITY.md` lo menciona)

## 9. Comunidad

- [ ] Hacé **fork** de un repo público que te guste y dale **star**
- [ ] Seguí (follow) a una organización
- [ ] Recorré el **Marketplace** y buscá la action `actions/checkout` que usa el workflow
- [ ] Leé qué es **GitHub Sponsors**

## Conceptos para repasar con Claude

- Git vs GitHub · GitHub Flow · fork vs clone vs template
- github.dev vs Codespaces · planes de Copilot · EMU (Enterprise Managed Users)
- InnerSource · roles de repo vs roles de organización
