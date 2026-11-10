# SM México · Un nuevo capítulo

Presentación interactiva para la conversación de Dirección General de SM México con la CEO Global. React, JavaScript, SVG y Vite. Diseño adaptado de la auditoría de redes SM indicada por el usuario: rojo SM, grises, Newsreader y Hanken Grotesk; logo tomado de ese sitio.

## Uso

Ocho vistas agrupadas en cinco capítulos. Navegación inferior, pestañas de capítulos o teclas izquierda/derecha. Modo presentación reduce la cabecera. Gráfica histórica con interruptor institucional, selección de año, porcentajes y tabla accesible. Mercado por segmento, reloj de arena seleccionable, capas de servicios e incentivos Smart/Core. Adaptación móvil y preferencia de movimiento reducido.

## Fuentes y límites

- `Plantilla y Cosper 2027.pptx`, diapositiva 1: cifras financieras y HC. Importes en millones de pesos. 2026 es forecast. El resultado disponible es **después de impuestos**. No hay una serie de resultado operativo en esta fuente.
- `Presentación 11 de Noviembre Oscar <> Marta.pptx`: diapositivas 14, 15, 41, 42, 46, 43, 34 y 35. Las diapositivas 14 y 15 se conservan completas en imágenes ampliables además de su adaptación interactiva.
- Datos de mercado: millones de euros, cierre del ciclo 2025–2026; estimaciones internas, sin verificación externa.
- El total 2026 se conserva en 439 aunque los componentes publicados suman 439.1 por redondeo. Los porcentajes usan el total publicado al incluir institucional, y la venta privada al excluirla. El resultado y HC mantienen el perímetro completo de la empresa.
- El rango de texto tradicional incluye del colegio y privado popular. Vivo SM 1.0 se mantiene como referencia adicional al total de soluciones 24.5. Idiomas publica 83.7 frente a una suma de componentes de 83.6.
- Crecimiento privado 2021–2026: 43.9%; HC: −26.0%; costo/venta privada: 50.8% a 42.6%. Se evitan multiplicadores y porcentajes de los titulares originales que no pueden reproducirse con las cifras redondeadas.
- 4,400+ servicios es una meta del plan. Asignación de asesores y cobertura son cambios previstos.
- La fuente contempla bonificaciones Smart/Core sin pesos ni fórmulas. Los criterios diferenciados se presentan como propuesta. El cierre de pertenencia es una recomendación narrativa, no un resultado medido.

## Desarrollo y publicación

```sh
npm ci
npm run dev
npm run build
```

Datos: `data.js`. Contenido e interacción: `src.jsx`. Estilos: `style.css`.
Cada push a main compila y publica `dist` mediante GitHub Actions en Pages. `base: './'` permite alojar bajo el nombre del repositorio. Los PPTX completos permanecen fuera del repositorio.
