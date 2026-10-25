# CréditoClaro

CréditoClaro es un simulador de crédito para una caja municipal peruana. Permite estimar cuotas mensuales por el método francés, revisar el cronograma de pagos, descargarlo en PDF y obtener una orientación referencial de elegibilidad.

## Problemática
En la entidad, el cliente no conoce cuota, costo total (TCEA) ni requisitos
hasta llegar a la agencia. Esto genera atenciones de 15 a 20 minutos solo para
explicar cálculos, visitas sin documentos completos y llamadas constantes para
consultar el estado del trámite.

## Usuario objetivo
- **Cliente potencial:** persona de 25 a 55 años con ingresos propios.
- **Asesor de créditos:** personal de agencia que recibe y evalúa solicitudes.

## Objetivo de la solución
Permitir que el cliente simule su crédito, verifique su elegibilidad preliminar,
registre una pre-solicitud y consulte su avance antes de acudir a la agencia.

## Funcionalidades principales
1. Simulador de crédito (cuota, interés total, TCEA, cronograma)
2. Verificador de elegibilidad preliminar
3. Checklist de requisitos según perfil
4. Registro de pre-solicitud con código de seguimiento
5. Seguimiento del trámite por código
6. Panel del asesor con filtros y cambio de estado

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

## Limitaciones
- Resultados referenciales, sin evaluación crediticia oficial.
- Los datos se guardan en el navegador (localStorage); no hay servidor.
