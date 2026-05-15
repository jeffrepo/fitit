# fititwork

Repositorio de personalizaciones Odoo para Fit It.

## Módulo `fitit_reports`

Addon para Odoo 19 que agrega formatos de reportes/cotizaciones basados en el machote 2026 de Fit It.

Formatos incluidos:

- Reporte de mantenimiento (`RPTE MMTO`).
- Bicicletas: contado + financiamiento.
- Bicicletas: renta compra.
- Compra MSI.
- Financiamiento equipo gym.

Formatos omitidos según requerimiento:

- Nota de remisión.
- Cotización contado.
- Cotización mantenimiento.
- Cotización evento.

El módulo extiende `sale.order` y `sale.order.line` con campos para datos del machote, contacto, observaciones, mantenimiento, flete, anticipo, valor residual, plazos e intereses. Los importes de financiamiento, renta y MSI se calculan automáticamente desde el total de la cotización y los parámetros capturados; para `BICIS: CONTADO+FINAN.` se pueden configurar los meses de financiamiento y el porcentaje de anticipo que se imprimen por producto.
