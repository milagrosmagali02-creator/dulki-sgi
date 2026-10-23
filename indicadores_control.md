## Indicadores de control y estándares de desempeño

Según el material de la cátedra (Unidad 4, Tema 1), el control administrativo permite garantizar que las actividades realizadas se ajusten a las planificadas, y se compone de cuatro etapas: establecimiento de estándares, medición del desempeño, comparación con lo esperado y corrección de los desvíos. Siguiendo ese esquema, defino a continuación los indicadores con los que se auditaría técnicamente el SGI de Dulkí S.A. en el proceso de reposición de stock. Los valores de los estándares (98 %, 24 h y 5 %) son propuestas propias, fijadas como umbrales razonables para la empresa ficticia.

| Indicador | Medición | Estándar | Frecuencia | Acción correctiva |
|---|---|---|---|---|
| Exactitud del stock calculado | % de artículos cuyo stock calculado coincide con el conteo físico | ≥ 98 % | Mensual | Revisar los movimientos y motivos del artículo |
| Cobertura de alertas (HU-01) | % de artículos bajo el stock mínimo que generaron alerta | 100 % | Semanal | Revisar la regla de cálculo y el stock_minimo |
| Tiempo de reacción (HU-02) | Horas entre la alerta y el pedido generado | ≤ 24 h hábiles | Semanal | Reasignar o escalar el pedido |
| Trazabilidad de ingresos (HU-03) | % de ingresos con artículo, depósito, proveedor y motivo completos | 100 % | Mensual | Corregir los registros incompletos |
| Mercadería no conforme | % de recepciones con reclamo al proveedor | ≤ 5 % | Mensual | Evaluar o cambiar de proveedor |

Cada indicador se vincula con una parte del proceso modelado en BPMN: la cobertura de alertas controla la primera compuerta ("¿Stock calculado < stock mínimo?"), el tiempo de reacción mide el tramo entre la alerta y el pedido, la trazabilidad de ingresos verifica el registro de la mercadería recibida y la tasa de mercadería no conforme controla la excepción de la segunda compuerta. La exactitud del stock calculado audita el cálculo en el que se apoya todo el sistema, definido en el diccionario de datos de la Entrega 3.