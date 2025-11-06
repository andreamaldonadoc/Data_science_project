# Golden Recovery

Prepara un prototipo de un modelo de machine learning para Zyfra. La empresa desarrolla soluciones de eficiencia para la industria pesada.

El modelo debe predecir la cantidad de oro extraído del mineral de oro. Dispones de los datos de extracción y purificación.

El modelo ayudará a optimizar la producción y a eliminar los parámetros no rentables.

## Proceso tecnológico

El mineral extraído se somete a un tratamiento primario para obtener la mezcla de mineral, o alimentación rougher, que es la materia prima utilizada para la flotación (también conocida como proceso rougher). Después de la flotación, el material se somete al proceso de purificación en dos etapas.

1. Flotación

La mezcla de mineral de oro se introduce en las plantas de flotación para obtener un concentrado de oro rougher y colas rougher (es decir, residuos del producto con una baja concentración de metales valiosos).

La estabilidad de este proceso se ve afectada por la volatilidad y el estado físico-químico desfavorable de la pulpa de flotación (una mezcla de partículas sólidas y líquido).

2. Purificación

El concentrado rougher se somete a dos etapas de purificación. Tras esto, tenemos el concentrado final y las nuevas colas.

## Descripción de datos

Rougher feed: materia prima
Rougher additions (o adiciones de reactivos): reactivos de flotación: xantato, sulfato, depresante
Xantato: promotor o activador de la flotación
Sulfato: sulfuro de sodio para este proceso en particular
Depresante: silicato de sodio
Rougher process: flotación
Rougher tails: residuos del producto
Float banks: instalación de flotación
Cleaner process: purificación
Rougher Au: concentrado de oro rougher
Final Au: concentrado de oro final
Parámetros de las etapas

air amount: volumen de aire
fluid levels
feed size: tamaño de las partículas de la alimentación
feed rate
Denominación de las características
Así es como se denominan las características:

[stage].[parameter_type].[parameter_name]

Ejemplo: rougher.input.feed_ag

Valores posibles para [stage]:

rougher: flotación
primary_cleaner: purificación primaria
secondary_cleaner: purificación secundaria
final: características finales
Valores posibles para [parameter_type]:

input: parámetros de la materia prima
output: parámetros del producto
state: parámetros que caracterizan el estado actual de la etapa
calculation: características de cálculo