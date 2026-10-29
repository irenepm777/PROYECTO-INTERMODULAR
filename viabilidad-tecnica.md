# Viabilidad técnica — SabiApp

## 1. Recursos tecnológicos necesarios

Planteamos SabiApp como una **aplicación web responsive**, de modo que funcione igual en ordenador, tablet o móvil sin que el usuario tenga que instalar nada. Para un público con poca experiencia digital, evitar la descarga desde una tienda de aplicaciones ya supone eliminar una barrera.

| Tecnología | Para qué la usamos en SabiApp |
|---|---|
| **HTML5, CSS3 y JavaScript** | Interfaz, diseño adaptable y ejercicios interactivos (arrastrar, seleccionar, completar formularios simulados). |
| **PHP** | Backend: registro e inicio de sesión, lógica de niveles, puntuaciones y recompensas. |
| **MySQL** | Base de datos con usuarios, lecciones, ejercicios, resultados y progreso. |
| **Git y GitHub** | Control de versiones, trabajo en ramas y revisión del código entre los tres. |
| **Docker** | Entorno de desarrollo idéntico para todo el equipo (servidor web, PHP y MySQL) y pruebas reproducibles. |
| **Figma** | Prototipos de pantallas y pruebas de navegación antes de programar. |
| **Lighthouse, WAVE y axe** | Comprobación de accesibilidad y rendimiento durante el desarrollo. |

Hemos elegido estas tecnologías porque son las que trabajamos en el ciclo, son gratuitas, cuentan con mucha documentación y se pueden alojar en casi cualquier servidor. La selección podrá ajustarse si durante el desarrollo vemos que alguna parte lo necesita.

Las funcionalidades que queremos cubrir con ellas son:

- **Aprendizaje por niveles**, con lecciones cortas que se desbloquean de forma progresiva.
- **Simulaciones de situaciones reales**, como pedir una cita médica, hacer una videollamada o detectar un mensaje fraudulento, siempre en un entorno ficticio.
- **Seguimiento del progreso**, para que el usuario (y, si lo desea, su familia o su centro) vea lo que ha avanzado.
- **Recompensas virtuales**, como insignias y logros, que animen a seguir practicando.

## 2. Materiales e infraestructura requerida

El proyecto no necesita instalaciones físicas especiales: todo el trabajo puede hacerse con equipos personales y servicios en la nube.

**Recursos materiales**

- Ordenadores personales para programar, diseñar y mantener la plataforma.
- Smartphones y tablets de distintos tamaños y gamas para probar la interfaz en condiciones reales, incluidos dispositivos antiguos o de gama baja, que son habituales entre nuestro público.
- Conexión a Internet para el desarrollo, las pruebas y el trabajo con el repositorio.

**Infraestructura digital**

- **Alojamiento web** compatible con PHP y MySQL (hosting compartido al principio y un servidor virtual si crece el número de usuarios).
- **Base de datos** para guardar la información y el progreso de los usuarios.
- **Dominio propio y certificado HTTPS**, imprescindible para proteger los datos de inicio de sesión.
- **Copias de seguridad automáticas** de la base de datos.
- **Entornos separados** de desarrollo, pruebas y producción, para no tocar nunca directamente la versión que usan los usuarios.

Durante el prototipado trabajaremos con entornos locales en Docker y herramientas gratuitas, así que la inversión inicial es prácticamente nula. Cuando pasemos a una versión pública tendremos que calcular el coste real de alojamiento, dominio, mantenimiento y seguridad, que se incluirá en el análisis económico.

## 3. Competencias técnicas del equipo

Somos tres estudiantes de 2.º de Desarrollo de Aplicaciones Web y durante el ciclo hemos trabajado programación, bases de datos, diseño de interfaces y despliegue de aplicaciones. Nos hemos repartido las responsabilidades técnicas según el área en la que cada uno se siente más fuerte, igual que en el organigrama:

| Integrante | Área | Responsabilidades |
|---|---|---|
| **Irene** | Desarrollo backend | Lógica de negocio en PHP, gestión de usuarios, niveles y progreso, y conexión con la base de datos. |
| **Baku** | Bases de datos e infraestructura | Diseño y administración de la base de datos, configuración de Docker y de los entornos, y despliegue. |
| **Juanma** | Desarrollo frontend | Interfaces y componentes visuales, adaptación responsive, interacción y navegación. |

Aunque cada uno lidera un área, usaremos GitHub para revisar el código de los demás, de modo que nadie sea el único que entiende una parte del proyecto.

Con lo que ya sabemos podemos desarrollar un prototipo funcional. Aun así, hay tres áreas en las que tendremos que investigar y formarnos más:

- **Accesibilidad avanzada:** aplicar las pautas WCAG 2.2 y adaptar el diseño a usuarios mayores (tamaño de texto, contraste, botones grandes, mensajes claros).
- **Seguridad en producción:** proteger la aplicación frente a las vulnerabilidades más habituales (por ejemplo, las del OWASP Top 10) y gestionar contraseñas y sesiones de forma segura.
- **Pruebas con usuarios reales:** preparar sesiones de prueba con personas mayores e interpretar los resultados para mejorar la plataforma.

## 4. Limitaciones técnicas identificadas

**Accesibilidad y usabilidad**

Nuestro público tiene niveles de experiencia tecnológica muy distintos y puede tener dificultades visuales, auditivas, motoras o cognitivas. Por eso la interfaz tiene que ser sencilla, con instrucciones claras, pocos pasos por pantalla y elementos fáciles de pulsar. No basta con que lo veamos nosotros: tendremos que comprobarlo con usuarios reales.

**Seguridad y protección de datos**

Vamos a guardar cuentas y datos de progreso, así que necesitamos autenticación segura, contraseñas cifradas y cumplir el RGPD y la LOPDGDD. Además, las simulaciones de bancos o administraciones públicas serán siempre ficticias: SabiApp nunca pedirá credenciales reales de esos servicios. Esto también sirve para enseñar al usuario a desconfiar de quien se las pida.

**Equipo reducido**

Con tres personas no podemos desarrollar todo a la vez. Tendremos que priorizar las funcionalidades principales en un producto mínimo viable (registro, lecciones interactivas, niveles y seguimiento del progreso) y dejar el resto para más adelante.

**Compatibilidad y conectividad**

La plataforma tiene que funcionar en distintos navegadores, tamaños de pantalla y dispositivos, incluidos los más antiguos o con conexiones lentas. Esto nos obliga a hacer páginas ligeras y a evitar efectos o librerías que no aporten nada.

**Mantenimiento de los contenidos**

Las aplicaciones y los trámites digitales cambian continuamente, y una lección puede quedarse desfasada en poco tiempo. Por eso queremos que las lecciones y simulaciones se guarden en la base de datos y se puedan editar desde un panel de administración, sin tener que tocar el código cada vez.

**Funcionalidades avanzadas**

La personalización con inteligencia artificial, los asistentes virtuales o la ayuda por voz son tendencias claras del sector, pero aumentan mucho la complejidad y el coste. Las reservamos para futuras versiones, cuando el funcionamiento básico esté validado.

## Fuentes de información

- [W3C. *Web Content Accessibility Guidelines (WCAG) 2.2*.](https://www.w3.org/TR/WCAG22/)
- [W3C WAI. *Older Users and Web Accessibility: Meeting the Needs of Ageing Web Users*.](https://www.w3.org/WAI/older-users/)
- [Reglamento (UE) 2016/679, Reglamento General de Protección de Datos (RGPD).](https://eur-lex.europa.eu/eli/reg/2016/679/oj)
- [Ley Orgánica 3/2018, de Protección de Datos Personales y garantía de los derechos digitales (LOPDGDD).](https://www.boe.es/eli/es/lo/2018/12/05/3/con)
- [Agencia Española de Protección de Datos (AEPD). Guías y herramientas.](https://www.aepd.es/)
- [OWASP Foundation. *OWASP Top 10*.](https://owasp.org/www-project-top-ten/)
- [MDN Web Docs (HTML, CSS y JavaScript).](https://developer.mozilla.org/es/)
- [Manual oficial de PHP.](https://www.php.net/manual/es/)
- [Documentación oficial de MySQL.](https://dev.mysql.com/doc/)
- [Documentación oficial de Docker.](https://docs.docker.com/)
- [Documentación oficial de Git.](https://git-scm.com/doc)
- [INE (2025). *Encuesta sobre equipamiento y uso de tecnologías de información y comunicación en los hogares*.](https://www.ine.es/)
- [ONTSI. *Uso de las tecnologías por las personas mayores en España*.](https://www.ontsi.es/)

## Resumen para la presentación (1 diapositiva)

**Viabilidad técnica**

- **Tecnología:** aplicación web responsive con HTML, CSS, JavaScript, PHP y MySQL; Git, Docker y Figma para desarrollar.
- **Infraestructura:** ordenadores, móviles y tablets de prueba; hosting, dominio con HTTPS y copias de seguridad. Prototipo con coste casi nulo.
- **Equipo:** Irene (backend), Baku (bases de datos e infraestructura) y Juanma (frontend). A reforzar: accesibilidad, seguridad y pruebas con usuarios.
- **Limitaciones:** accesibilidad para mayores, protección de datos (RGPD), equipo reducido, dispositivos antiguos y contenidos que cambian. La IA queda para versiones futuras.