## Ejemplo de errores al usar `git commit --amend`

A continuación se muestran imágenes de errores comunes al intentar usar `git commit --amend` en Git.

### Primer error al intentar hacer amend

![Error al hacer amend](https://i.ibb.co/Ld38ZgHH/Captura-de-pantalla-2025-08-19-104607.png)

Este error puede ocurrir si intentas hacer un `amend` en una situación donde no hay cambios para modificar el último commit, o si hay algún conflicto con el estado del repositorio.

### Segundo error relacionado con amend

![Otro error de amend](https://i.ibb.co/Q7mT3mhN/Captura-de-pantalla-2025-02-28-133350.png)

En este caso, el error puede estar relacionado con el estado del área de staging o con la configuración del repositorio.

---

Cuando envíes tu código, reemplazaré los datos de ejemplo por los tuyos.

## Guía visual: Desarrollo con 4 ramas (`html`, `js`, `css` y `main`) y commits con Conventional Commits

A continuación se muestra una guía paso a paso, con imágenes, sobre cómo trabajar en un repositorio Git con cuatro ramas principales y realizar commits siguiendo el estándar [Conventional Commits](https://www.conventionalcommits.org/).

### 1. Crear y visualizar las ramas

```bash
git branch html
git branch js
git branch css
git branch main
git branch
```

![Visualizar ramas](https://i.ibb.co/0Jw8kQJ/git-branch-list.png)

### 2. Cambiar a una rama y realizar cambios

Por ejemplo, para trabajar en la rama `html`:

```bash
git checkout html
```

![Cambiar de rama](https://i.ibb.co/6rQw3wY/git-checkout-html.png)

Realiza tus cambios en los archivos correspondientes.

### 3. Añadir cambios al área de staging

```bash
git add index.html
```

![Agregar archivos al staging](https://i.ibb.co/3yJkQwT/git-add-html.png)

### 4. Hacer un commit usando Conventional Commits

Ejemplo de mensaje de commit:

```bash
git commit -m "feat(html): agregar estructura básica de la página"
```

![Commit convencional](https://i.ibb.co/4Vw8w2y/git-commit-conventional.png)

### 5. Repetir el proceso en otras ramas

Cambia a las ramas `js` y `css` para realizar cambios específicos y haz commits siguiendo el mismo formato:

- `feat(js): agregar lógica de validación`
- `feat(css): añadir estilos principales`

### 6. Fusionar ramas en `main`

Cuando las ramas estén listas, cámbiate a `main` y fusiona los cambios:

```bash
git checkout main
git merge html
git merge js
git merge css
```

![Fusión de ramas](https://i.ibb.co/7Qw8kQJ/git-merge-main.png)

---

Esta guía te ayudará a mantener un flujo de trabajo organizado y mensajes de commit claros y consistentes.