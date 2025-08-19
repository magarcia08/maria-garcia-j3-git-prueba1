## Ejemplo de errores al usar `git commit --amend`

A continuación se muestran imágenes de errores comunes al intentar usar `git commit --amend` en Git.

### Primer error al intentar hacer amend

![Error al hacer amend](https://i.ibb.co/TnYwdHy/Captura-de-pantalla-2025-08-19-104607.png)

Este error puede ocurrir si intentas hacer un `amend` en una situación donde no hay cambios para modificar el último commit, o si hay algún conflicto con el estado del repositorio.

### Graph

![Graph de lo sucedido](https://i.ibb.co/fWhXhbh/Captura-de-pantalla-2025-08-19-104712.png)


## Guía visual: Desarrollo con 4 ramas (`html`, `js`, `css` y `main`) y commits con Conventional Commits

A continuación se muestra una guía visual del flujo de trabajo usando cuatro ramas principales y mensajes de commit siguiendo el estándar [Conventional Commits](https://www.conventionalcommits.org/).

### 1. Creación de ramas

Cada rama representa una parte del proyecto:

- `html` para la estructura.
- `css` para los estilos.
- `js` para la lógica.
- `main` para integración y despliegue.

### Ejemplo de diagrama de ramas

A continuación se muestra un diagrama ilustrativo de cómo pueden organizarse las ramas en un proyecto Git:

![Diagrama de ramas](https://i.ibb.co/Q3xJwrb0/Captura-de-pantalla-2025-08-19-110328.png)

### 2. Realización de commits siguiendo Conventional Commits

Ejemplo de mensajes de commit:

- `feat(html): agregar estructura básica de la página`
- `style(css): mejorar el diseño del encabezado`
- `fix(js): corregir error en validación de formulario`

![Ejemplo de commit](https://i.ibb.co/PzYhgVWP/Captura-de-pantalla-2025-08-19-110435.png)

### 3. Fusión de ramas a `main`

Una vez completados los cambios en cada rama, se realiza un merge a `main` asegurando que los mensajes de commit sean claros y descriptivos.

![Merge de ramas](https://i.ibb.co/sJdCtc5B/Captura-de-pantalla-2025-08-19-110532.png)

---

Esta metodología facilita la colaboración y el mantenimiento del proyecto, asegurando un historial de commits limpio y comprensible.