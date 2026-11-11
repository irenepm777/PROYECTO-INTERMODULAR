# Presupuesto y Financiación: SabiApp

* **Módulo:** Proyecto Intermodular (2.º DAW)
* **Sprint 2:** Estructuración y Planificación (RA2.h Presupuesto económico)
* **Equipo de Desarrollo:** Minority Report (Juan Manuel Francisco Mendoza, Bakunin Sosa Álvarez, Irene Pascual Moreno)
* **Fecha:** Noviembre 2026

---

## Resumen

Llevar SabiApp hasta un MVP funcional, lanzarlo y mantenerlo durante un año cuesta unos **893 €** de desembolso real (≈ 298 € por persona): todo el software es gratuito y el equipo ya dispone de ordenadores, así que los gastos relevantes son los dos dispositivos de prueba (310 €) y el marketing de lanzamiento (275 €). Según el modelo de ingresos del pitch, **una sola licencia de centro** (o unas 16 suscripciones durante un año) cubre ese presupuesto completo.

---

## 1. Presupuesto de costes directos

Horizonte: desarrollo del MVP + 12 meses de servicio. Importes en euros, IVA incluido.

| Categoría | Partida | Cálculo | Coste |
| :--- | :--- | :--- | ---: |
| **Material y equipamiento** | Equipos de desarrollo | 3 portátiles propios, ya disponibles | 0,00 € |
| | Smartphone Android de gama básica (pruebas) | 1 ud. | 150,00 € |
| | Tablet Android de gama básica (pruebas) | 1 ud. | 160,00 € |
| | Material fungible (guiones de prueba, consentimientos, papel) | Estimación | 25,00 € |
| **Licencias de software** | PHP, MySQL, Docker, Git/GitHub, Figma Education, Lighthouse, WAVE, axe DevTools, Let's Encrypt, tipografía Lexend | Gratuitas o de código abierto | 0,00 € |
| **Servicios externos** | VPS con copias de seguridad | ≈ 10 €/mes × 12 | 120,00 € |
| | Dominio `.es` | Primer año | 7,25 € |
| | Sesiones de prueba con personas mayores (merienda de agradecimiento) | ≈ 10 participantes × 4 € | 40,00 € |
| | Subcontrataciones | Ninguna: el equipo cubre frontend, backend, BBDD y DevOps | 0,00 € |
| **Marketing y lanzamiento** | Piezas gráficas (flyers, redes, presentación) con Canva | Plan gratuito | 0,00 € |
| | Flyers A5 para centros de mayores y asociaciones | 500 ud. | 84,70 € |
| | Publicidad en Meta Ads (Facebook/Instagram) dirigida a familias de 35-55 años | 50 €/mes × 3 meses | 150,00 € |
| | Visitas y demos en centros de mayores (desplazamientos) | ≈ 10 visitas × 4 € | 40,00 € |
| | Vídeo demo y redes sociales | Móvil propio y edición gratuita; la web usa el dominio ya presupuestado | 0,00 € |
| | **Subtotal marketing** | | **274,70 €** |
| | **Subtotal costes directos** | | **776,95 €** |
| **Contingencia** | 15 % para desviaciones de precio, ampliación del servidor, coste real de la publicidad o reposición de dispositivos | 776,95 € × 0,15 | 116,54 € |
| | **TOTAL** | | **893,49 €** |

* **Por qué 15 % y no 10 %:** las partidas más inciertas son el servidor (el plan de referencia de Hetzner, CX22 a 3,79 €/mes, figura ya como obsoleto) y el coste real por clic de la publicidad.
* **Marketing:** lo lleva Juanma (marketing, según el organigrama del pitch). Los 150 € de anuncios dan ≈ 250 clics (CPC medio de Facebook ≈ 0,63 $, ≈ 0,6 €; no hay dato específico para España): valen para validar el mensaje, no para escalar. La captación principal va por canal directo (centros de mayores y asociaciones), que cuesta tiempo y no dinero.
* **Escenario mínimo:** con dispositivos reacondicionados o cedidos por un centro de mayores (−310 €), el total baja a ≈ **537 €** (≈ 179 € por persona).
* **RGPD sin coste:** la documentación básica se genera con *Facilita RGPD* de la AEPD, gratuita y válida para tratamientos de bajo riesgo; SabiApp no recoge datos sanitarios ni bancarios reales.

---

## 2. Coste del trabajo del equipo (no desembolsado)

El Team Charter fija 8-10 h/semana por persona. Con 9 h, son 27 h/semana; valoradas a 15 €/h (tarifa junior supuesta), ≈ **405 €/semana**, unos **4.860 €** en un desarrollo de 12 semanas (duración supuesta). No sale de caja, pero es el coste real si hubiera que contratar ese trabajo.

---

## 3. Financiación

**Responsables (según el organigrama del pitch):** compras, Bakunin; contabilidad y gestión financiera, Irene y Juanma.

* **Fase MVP:** aportación del equipo a partes iguales (≈ 298 € por persona, ≈ 179 € en el escenario mínimo). Sin deuda ni inversores externos.
* **Apoyo en especie:** stakeholders y centros piloto pueden ceder personas y espacio para las pruebas con mayores, y dispositivos (a negociar). Reduce el presupuesto sin aportar dinero.
* **Tras el MVP:** ingresos propios del modelo *freemium*: suscripción de 5 €/mes y licencia de centro de 100 €/mes. Las ayudas a la inclusión digital se explorarán más adelante y no se cuentan en este presupuesto.

---

## 4. Viabilidad económica

* **Escenario del pitch:** 200 suscripciones × 5 € × 12 + 10 centros × 100 € × 12 = 12.000 € + 12.000 € = **24.000 €/año**.
* **Costes recurrentes tras el MVP:** ≈ 128 €/año (servidor con copias, 120 €, y renovación del dominio, 8,46 €), más la publicidad que se decida mantener (referencia: 50 €/mes).
* **Comisión de cobro** (Stripe, tarjetas del EEE: 1,5 % + 0,25 € por cobro): una suscripción de 5 € pierde ≈ 0,33 € (6,5 %); una licencia de 100 €, ≈ 1,75 € (1,75 %). Con un plan anual de 60 € la comisión baja a 1,15 € (1,9 %), por lo que conviene ofrecerlo.
* **Punto de equilibrio:** una licencia de centro (1.200 €/año) cubre el presupuesto completo; solo con suscripciones, hacen falta ≈ 16 suscriptores durante un año.
* **Cautela:** los 24.000 € son un escenario hipotético por validar (próximo paso del pitch: validación con usuarios y análisis económico). Alcanzar ≈ 210 clientes no es realista solo con 150 € de anuncios: depende de alianzas con centros y del boca a boca, y el presupuesto de marketing debe revisarse tras validar. Tampoco incluyen impuestos, forma jurídica ni salarios.

---

## Supuestos y fuentes

Precios consultados el 10/11/2026. Son estimaciones propias: material fungible, merienda de las pruebas, 10 €/mes de VPS con copias, 4 € por visita a centros, 3 meses de anuncios a 50 €/mes, 15 €/h de tarifa y 12 semanas de duración.

* Equipo, horas y roles: [Team Charter](./Contrato-grupal.pdf) y [Pitch del sector](./Pitch-sector-SabiApp.pdf) (organigrama y modelo de ingresos).
* Dominio `.es`: [OVHcloud](https://www.ovhcloud.com/es-es/domains/tld/es/) (5,99 € sin IVA el primer año; 6,99 € de renovación).
* Servidor de referencia: [Hetzner CX22 en VPS Benchmarks](https://vpsbenchmarks.com/hosters/hetzner/plans/cx22) (3,79 €/mes, plan obsoleto).
* Tablet: [Lenovo Tab M11, oferta ≈ 160 €](https://www.elgrupoinformatico.com/tablets/oferta-lenovo-tablet-tab-m11/).
* Smartphone: [móviles baratos en Xataka](https://www.xataka.com/seleccion/mejores-moviles-baratos) (de 111 € a 170 €; Moto G06 Power desde 149 €).
* Figma gratis para estudiantes: [Figma Education](https://www.figma.com/education/students/).
* RGPD: [Facilita RGPD (AEPD)](https://www.aepd.es/guias-y-herramientas/herramientas/facilita-rgpd).
* Comisiones de cobro: [Stripe](https://stripe.com/es/pricing).
* Publicidad: [CPC medio de Facebook Ads, Influee (jul. 2026)](https://influee.co/es/blog/good-cpc-facebook-ads) (0,63 $; sin dato para España).
* Flyers: [MOO, 500 flyers A5](https://www.moo.com/es/flyers/a5) (84,70 €).