# Aspectos Innovadores y Comparativa del Proyecto: SabiApp

* **Módulo:** Proyecto Intermodular (2º DAW - ILERNA)
* **Sprint 1:** Descubrimiento y Definición
* **Equipo:** Juanma, Baku, Irene (Minority Report)

---

## 1. ¿Qué hace diferente a SabiApp?.

Cuando investigamos qué aplicaciones y servicios existen hoy en el mercado para personas mayores, nos dimos cuenta de que hay un hueco enorme que nadie está cubriendo bien:

* Por un lado están aplicaciones como **Lumosity** o **CogniFit**, que tienen juegos de memoria o agilidad mental (como recordar secuencias de colores o cartas). Están bien para ejercitar la mente, pero **no te enseñan a pedir una cita médica, a usar Bizum o a enviar una foto por WhatsApp**.
* Por otro lado están plataformas de idiomas como **Duolingo**, que tienen un sistema muy bueno de lecciones cortas y motivación diaria, pero están pensadas solo para aprender lenguas y para un público general.
* Y por último existen iniciativas como **Bleta** o **Canal Sénior**, que venden tablets adaptadas bastante caras o hacen charlas por videollamada, pero no ofrecen una aplicación interactiva en la web o en el móvil propio del usuario donde pueda practicar paso a paso.

Nuestra idea con **SabiApp** es coger lo mejor del método de lecciones diarias de Duolingo y aplicarlo a la **enseñanza de tareas digitales reales**, creando una aplicación diseñada desde cero pensando exclusivamente en las necesidades de una persona mayor.

```
                    [ Diseñado específicamente para mayores ]
                                       ▲
                                       │          ★ SabiApp
                                       │        (Nuestro hueco)
                   CogniFit            │
                                       │     Canal Sénior
   Juegos mentales                     │                       Aprender a usar
   abstractos      ◄───────────────────┼─────────────────────► apps y trámites
   (memoria, etc.)                     │                       reales del día a día
                                       │
                   Lumosity            │     Duolingo
                                       ▼
                       [ Para todo tipo de público ]
```

---

## 2. Los cuatro puntos innovadores de SabiApp

Para que el proyecto sea sólido y viable desde el punto de vista técnico y de diseño, hemos dividido la innovación en cuatro partes:

### 1. Tecnología: Práctica en simuladores seguros (modo de pruebas o *sandbox*)

* En lugar de enseñar con vídeos aburridos o textos largos, en SabiApp el usuario aprende **tocando en pantallas interactivas que simulan ser aplicaciones reales** (un simulador de WhatsApp, un simulador de Bizum, la app del banco o la web de citas de su médico).
* Estas pantallas funcionan como un «cajón de arena» de pruebas (*sandbox*): el saldo de dinero es inventado, los contactos son simulados y el entorno está aislado. Si el usuario pulsa un botón incorrecto o se confunde de número, **no pasa absolutamente nada**. No puede perder dinero, no puede romper nada ni borrar datos reales. La app le explica con calma qué ha pasado y le permite volver a probar tantas veces como necesite.
* Incluimos lecciones prácticas para **aprender a detectar estafas**: les mostramos ejemplos interactivos de SMS sospechosos o correos falsos para que aprendan a fijarse en los detalles antes de pinchar en enlaces peligrosos.

### 2. Diseño y experiencia de usuario (adaptado 100% a mayores)

* **Facilidad de lectura:** Usamos fuentes tipográficas muy limpias y legibles (*Lexend* y *Plus Jakarta Sans*), pensadas para personas con vista cansada. El tamaño de letra es grande y los colores tienen un contraste muy alto para que no cueste distinguir los textos de los fondos.
* **Botones amplios y cómodos:** Las zonas donde hay que pulsar en la pantalla son grandes (mínimo de 48 a 56 píxeles de alto), lo que facilita el uso a personas con problemas de movilidad o temblor en las manos.
* **Lenguaje sencillo:** No utilizamos términos informáticos en inglés ni palabras técnicas que desorienten (evitamos palabras como *login*, *scroll*, *feedback* o *swipe*). Todas las explicaciones están redactadas en un lenguaje cotidiano y cercano.

### 3. Metodología de aprendizaje: Gamificación sin castigos

* Aplicamos dinámicas de juego (lo que técnicamente se llama *gamificación*): lecciones muy cortas de unos 3 a 5 minutos (*microlearning*), seguimiento de días seguidos practicando (rachas) y sonidos y animaciones alegres cuando completan una tarea.
* **Sin estrés ni penalizaciones:** En aplicaciones como Duolingo, si te equivocas varias veces «pierdes vidas» y la app te bloquea o te hace pagar. En SabiApp hemos eliminado cualquier tipo de castigo: no hay cuentas atrás con temporizadores que pongan nerviosa a la persona, no se pierden vidas y el usuario puede repetir el ejercicio tantas veces como quiera. Lo que premiamos es la constancia y las ganas de aprender.

### 4. Modelo de negocio y aplicación práctica

* **Para personas individuales (modelo mixto o *freemium*):** La aplicación se puede descargar gratis con lecciones básicas para aprender lo fundamental. Quien quiera módulos avanzados o soporte preferente tiene una suscripción muy asequible (unos 5 € al mes).
* **Para centros y ayuntamientos:** Ofrecemos licencias para centros de día, asociaciones de vecinos o residencias (aproximadamente 100 € al mes por centro). Esto les incluye acceso completo para sus alumnos y un panel de control donde los monitores pueden ver cómo progresa cada persona en el taller de informática.

---

## 3. Tabla comparativa con las alternativas existentes

| Característica                        | Lumosity / CogniFit                 | Duolingo                          | Bleta / Canal Sénior                          | SabiApp                                                                        |
| :------------------------------------- | :---------------------------------- | :-------------------------------- | :--------------------------------------------- | :----------------------------------------------------------------------------- |
| **¿Para quién es?**            | Todo tipo de público               | Quien quiera aprender idiomas     | Mayores (formato clásico)                     | **Mayores (55 a 75+ años)**                                             |
| **¿Qué te enseña?**           | Memoria y agilidad mental abstracta | Vocabulario e idiomas             | Charlas generales o tablet con apps básicas   | **Trámites y apps del día a día (banco, salud, Bizum, WhatsApp)**     |
| **¿Cómo se aprende?**          | Minijuegos repetitivos              | Ejercicios de rellenar y traducir | Clases por vídeo o cursos presenciales        | **Simuladores prácticos guiados paso a paso**                           |
| **¿Qué pasa si te equivocas?** | Pierdes puntuación                 | Pierdes vidas y te bloquea        | Tienes que volver a preguntar al profesor      | **Nada: no hay vidas, no hay prisa y puedes repetir siempre**            |
| **¿Dónde se usa?**             | Móvil / Ordenador                  | Móvil / Ordenador                | En su tablet específica o en el PC del centro | **En el propio móvil que la persona ya tiene en el bolsillo/Ordenador** |

---

## 4. Fuentes de información

* **Análisis de plataformas y competidores de referencia:**
  * Metodología de *microlearning* y gamificación: modelo pedagógico y de retención de **Duolingo**.
  * Aplicaciones de estimulación cognitiva: plataformas de entrenamiento mental **CogniFit** y **Lumosity**.
  * Soluciones existentes para mayores: análisis de producto y hardware de **Bleta** y plataforma de cursos telemáticos **Canal Sénior**.
* **Pautas de diseño y accesibilidad web (UX/UI):**
  * **W3C / WAI:** *Web Content Accessibility Guidelines* (WCAG 2.1 / 2.2, niveles AA y AAA) para ratio de contraste de color, legibilidad y navegación accesible.
  * **Google Material Design & Apple Human Interface Guidelines (HIG):** Especificaciones de diseño para personas con motricidad reducida (dimensiones mínimas de objetivos táctiles de 48x48 dp / 44x44 pt).
  * **Investigación tipográfica:** Fundamentos de legibilidad de la tipografía *Lexend* (diseñada para facilitar la fluidez lectora) y *Plus Jakarta Sans*.
* **Pedagogía y dinámicas de interacción:**
  * Estudios sobre aprendizaje en adultos mayores y gamificación no punitiva (*positive reinforcement* frente a sistemas de penalización por vidas o tiempo limitado).
* **Estudios de mercado e impacto económico:**
  * Informes de la Comisión Europea sobre la *Silver Economy* (economía plateada) y servicios de digitalización inclusiva para el envejecimiento activo.

---

## 5. Resumen para la diapositiva de presentación

* **Propuesta clave:** Primera aplicación que enseña a personas mayores a desenvolverse con su móvil mediante simulaciones interactivas y seguras de apps reales.
* **Diferenciación principal:** En lugar de juegos mentales o cursos teóricos, ofrecemos práctica directa en un entorno seguro donde es imposible equivocarse o perder dinero.
* **Diseño accesible:** Tipografía grande, botones anchos, contraste alto y lenguaje sin tecnicismos.
* **Metodología:** Lecciones cortas y motivadoras sin cronómetros ni penalizaciones.
