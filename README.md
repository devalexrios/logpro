# logpro

Una sencilla adición a `git` que llega en forma de **alias**, `git logpro` es un **log** personalizado que me gustaría compartir con ustedes.

## Demostración

![Imagen demostrativa](screenshot-demo.png)

## Implementación

Abre la configuración global de Git con:

```bash
git config --global -e
```

Y pega el siguiente contenido al final del fichero que se te abrió.

```conf
[alias]
	logpro = log '--pretty=format:%C(bold cyan)%h%Creset ← %C(bold italic)%an%Creset → %C(bold green)%cr%Creset %C(bold yellow)// %s%Creset%C(bold magenta)%d%Creset' --graph
```

## Uso

Ejecute `git logpro` y vea las diferencias. 😃️
