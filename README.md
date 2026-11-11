# SM México · Un nuevo capítulo

Presentación interactiva para la conversación de Dirección General de SM México con la CEO Global. React, JavaScript, SVG y Vite. Diseño adaptado de la auditoría de redes SM indicada por el usuario: rojo SM, grises, Newsreader y Hanken Grotesk; logo tomado de ese sitio.

## Uso

Doce vistas agrupadas en seis capítulos. Navegación inferior, pestañas de capítulos o teclas izquierda/derecha. Modo presentación reduce la cabecera. Gráfica histórica única con cinco interruptores independientes: venta privada, institucional, costo relativo, personas y resultado después de impuestos. Selector separado de base del costo (venta total o privada), selección de año y tabla accesible. Mercado por segmento, reloj de arena seleccionable, capas de servicios e incentivos Smart/Core. Adaptación móvil y preferencia de movimiento reducido.

## Operación

Capítulo añadido a partir de información proporcionada por el usuario: comités de Dirección, Negocio, LIJ, Compras, Operaciones y Tecnología, cada uno con frecuencias, KPIs y responsables establecidos. No se asignan periodicidades concretas, indicadores específicos ni nombres que no se hayan proporcionado.

## Fuentes y límites

- `Plantilla y Cosper 2027.pptx`, diapositiva 1: cifras financieras y HC. Importes en millones de pesos. 2026 es forecast. El resultado disponible es **después de impuestos**. No hay una serie de resultado operativo en esta fuente.
- `Presentación 11 de Noviembre Oscar <> Marta.pptx`: diapositivas 14, 15, 41, 42, 46, 43, 34 y 35. Las diapositivas 14 y 15 se conservan completas en imágenes ampliables además de su adaptación interactiva.
- Datos de mercado: millones de euros, cierre del ciclo 2025–2026; estimaciones internas, sin verificación externa.
- El total 2026 se conserva en 439 aunque los componentes publicados suman 439.1 por redondeo. Los porcentajes usan la base seleccionada (total publicado o venta privada), independiente de la visibilidad de las series. El resultado y HC mantienen el perímetro completo de la empresa.
- El rango de texto tradicional incluye del colegio y privado popular. Vivo SM 1.0 se mantiene como referencia adicional al total de soluciones 24.5. Idiomas publica 83.7 frente a una suma de componentes de 83.6.
- Crecimiento privado 2021–2026: 43.9%; HC: −26.0%; costo/venta privada: 50.8% a 42.6%. Se evitan multiplicadores y porcentajes de los titulares originales que no pueden reproducirse con las cifras redondeadas.
- 4,400+ servicios es una meta del plan. Asignación de asesores y cobertura son cambios previstos.
- La compensación SMART y CORE se detalla en tres vistas adicionales basadas en SIMPLE Compensación variable comercial 2027. Se distinguen pesos, umbrales, evidencias y condiciones; el cierre de pertenencia es una recomendación narrativa, no un resultado medido.

## Desarrollo y publicación

```sh
npm ci
npm run dev
npm run build
```

Datos: `data.js`. Contenido e interacción: `src.jsx`. Estilos: `style.css`.
Cada push a main compila y publica `dist` mediante GitHub Actions en Pages. `base: './'` permite alojar bajo el nombre del repositorio. Los PPTX completos permanecen fuera del repositorio.

## Pantalla de acceso

Acceso visual mediante contraseña, con verificación SHA-256 en el navegador y sesión por pestaña. La contraseña no se guarda en texto plano en el código. Este bloqueo cliente no protege el código, las imágenes ni los datos públicos de GitHub Pages; no constituye autenticación de servidor.

## Captura ilustrativa de comités

`public/assets/comites-tablero-simulado.png` es una captura de una reproducción local del tablero, construida con su estructura visual observada, su CSS y su logo públicos. Todos los indicadores, estados y porcentajes fueron sustituidos por información simulada. Se omiten perfiles personales y comités fuera del alcance de la presentación. No se modificaron registros en PRO-Comités SM.

## Compensación variable 2027

Síntesis de 22 diapositivas en tres vistas adicionales: SMART (1–10), CORE (11–17), aceleradores y condiciones (18–22). SMART es 10% y CORE 20% del sueldo anual cobrado según diapositivas 1, 9 y 17; la expresión “10% del bono” de la diapositiva 2 se interpreta con esas bases explícitas. Ejemplo SMART: la fuente paga $26,375 tras redondeo intermedio; sin ese redondeo resulta $26,385, diferencia mostrada en el detalle. Escala de visitas conserva “>80%”; el 80% exacto y la precisión de los intervalos quedan sin resolver. No se ofrece calculadora de nómina. Abril de 2028 para CORE, aceleradores y premios fue confirmado expresamente por el usuario.
