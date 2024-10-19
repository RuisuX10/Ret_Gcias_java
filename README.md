# Proyecto de Cálculo de Retención

Este proyecto en Java tiene como objetivo calcular la retención basada en diferentes tipos de conceptos, como bienes muebles, servicios y alquileres.

## Estructura del Proyecto

El proyecto consta de dos partes principales:

1. **Método de cálculo de retención**:
   ```java
   public float calcularRetencion(float neto, float noImponible, float alicuota, boolean retAnt) {
       float retencion = retAnt ? neto * alicuota : (neto - noImponible) * alicuota;
       return retencion;
   }
