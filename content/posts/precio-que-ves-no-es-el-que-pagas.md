+++
title = 'El precio que ves no es el que pagas: moneda local, spread y comisiones'
date = '2026-09-06T08:20:00-06:00'
draft = false
tags = ['precios', 'moneda', 'tiendas']
summary = 'Un agregador reportaba 3.94 USD. La tienda cobraba el equivalente a 5.33 USD. Más de 25% de diferencia, antes de que tu tarjeta cobre lo suyo.'

[cover]
  image = 'images/covers/precio-real.svg'
  alt = 'Icono de intercambio de divisas con símbolo de dólar'
  relative = false
+++

Los comparadores de precios suelen mostrar todo en dólares para que sea fácil comparar entre tiendas. El problema es que ese número no siempre es el que vas a pagar, y la diferencia puede ser grande.

## Un caso real

El juego PEAK, en la tienda AllYouPlay:

| Fuente | Precio mostrado |
|---|---|
| IsThereAnyDeal (reportado) | 3.94 USD |
| AllYouPlay (precio real en tienda) | 89.99 MXN |
| Equivalente en USD al tipo de cambio del día | ~5.33 USD |
| Diferencia frente al precio reportado | Más de 25% |

El agregador no mentía ni estaba desactualizado: simplemente reportaba una conversión de referencia, mientras la tienda cobra en moneda local a su propio tipo de cambio, que no tiene por qué coincidir con el de mercado.

![Ficha de PEAK en AllYouPlay mostrando el precio $89.99 y "Se activa en México"](/blogdeofertas/images/screenshots/allyouplay-peak-precio-mxn.png "AllYouPlay cobra en pesos mexicanos, mientras el agregador reportaba 3.94 USD para el mismo juego")

Nada en la ficha del producto avisa de la diferencia: el precio se ve normal, confirmado además por la etiqueta de activación en México. Solo se nota si ya traías el dato del agregador en la cabeza y haces la conversión tú mismo.

Esto no es un caso aislado de AllYouPlay. GreenManGaming, por ejemplo, cotiza directamente en pesos mexicanos sin que haga falta convertir nada:

![Ficha de Final Fantasy XIV Online Starter Edition en GreenManGaming mostrando el precio $360 MXN](/blogdeofertas/images/screenshots/greenmangaming-ffxiv-precio-mxn.png "GreenManGaming muestra el precio directamente en pesos mexicanos, su propia conversión desde el precio base")

El punto no es que cotizar en moneda local esté mal — al contrario, suele ser más claro que mostrar dólares. El punto es que ese número en pesos ya incluye el tipo de cambio que decidió la tienda, no el que reportó el agregador ni el de mercado, y ahí es donde aparece la diferencia.

## Por qué pasa esto

**El tipo de cambio de la tienda es suyo, no el de referencia.** Cada tienda decide a qué tipo de cambio convierte sus precios a moneda local, y ese tipo puede tener un margen incorporado frente al tipo de cambio de mercado.

**El tipo de cambio de referencia tampoco es el de tu banco.** El tipo de cambio del Banco Central Europeo (u otro de referencia) que usan muchos agregadores no es el que aplica tu banco o tu tarjeta al momento de cobrar la compra. Entre el spread cambiario propio del banco y la comisión por transacción internacional, en México es común terminar pagando entre 1.5% y 3.5% más sobre el monto convertido.

Estos dos efectos se suman: el precio que ves en el agregador, el precio que muestra la tienda en tu moneda, y el cargo final en tu estado de cuenta pueden ser tres números distintos.

## Cómo protegerte

- **No decidas con el precio del agregador.** Úsalo solo para ubicar candidatas; el precio real está en la página de pago de la tienda, en tu moneda.
- **Revisa el precio en moneda local antes de confirmar el pago**, no el que aparece convertido a USD en la lista de resultados.
- **Considera la comisión de tu propia tarjeta o banco por compras internacionales.** Si tu tarjeta cobra comisión por transacciones en el extranjero o en moneda distinta, ese costo se suma después de que la tienda ya te cobró su tipo de cambio.
- **Compara el total final, no el precio de catálogo**, cuando estés decidiendo entre dos tiendas con precios parecidos.

## Lo que conviene recordar

"Precio en dólares" es una simplificación útil para comparar rápido, pero no es el número que vas a pagar. En el caso de PEAK, esa simplificación convirtió un precio anunciado de 3.94 USD en un cobro real de 89.99 MXN (~5.33 USD) — antes de que tu tarjeta sume, encima, su propia comisión por compra internacional. La próxima vez que un agregador te muestre un precio en dólares, revisa el precio en tu moneda dentro de la tienda antes de decidir: es el único de los dos que realmente vas a pagar.
