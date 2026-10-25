# CréditoClaro

CréditoClaro es un simulador de crédito para una caja municipal peruana. Permite estimar cuotas mensuales por el método francés, revisar el cronograma de pagos, descargarlo en PDF y obtener una orientación referencial de elegibilidad.

## Ejecutar localmente

La aplicación es un sitio estático de un solo archivo y no requiere instalar dependencias ni compilarlo.

1. Descarga o clona este repositorio.
2. Abre `index.html` directamente en un navegador moderno.

Opcionalmente, puedes servir la carpeta con Python:

```bash
python -m http.server 8000
```

Luego abre <http://localhost:8000>.

## Publicación

GitHub Actions valida el HTML en los pull requests y publica `index.html` en GitHub Pages cuando los cambios llegan a `main`.

Las cuotas y la evaluación de elegibilidad son estimaciones referenciales; no constituyen una oferta ni una aprobación de crédito.
