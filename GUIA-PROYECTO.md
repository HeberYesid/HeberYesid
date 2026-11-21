# Perfil de GitHub

Repositorio de presentación pública en GitHub. Su producto es un README con secciones de perfil, métricas, tecnologías, proyectos y enlaces; no es una aplicación web autónoma.

## Componentes y flujo

[`README.md`](README.md) es la entrada renderizada por GitHub. [`assets/`](assets/) guarda la cabecera y gráficos. La cabecera incluye una variante estática para preferencias de movimiento reducido. [`.github/workflows/snake.yml`](.github/workflows/snake.yml) declara la generación del gráfico de contribuciones y el guardado de `assets/snake.svg` en el repositorio; el README muestra ese recurso.

El visitante abre el perfil → GitHub renderiza el Markdown → el navegador muestra los recursos declarados y permite seguir los enlaces. La generación de la animación ocurre fuera de la visita; no hay base de datos local ni proceso de servidor que iniciar.

## Uso y lectura

Lee `README.md`, luego revisa `assets/` y por último `snake.yml` si quieres entender la actualización automática. Para revisar localmente basta un visor Markdown; este no necesariamente reproduce las reglas exactas de GitHub. No se comprobó la actividad del workflow remoto.
