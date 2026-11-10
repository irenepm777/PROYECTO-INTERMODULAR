Diagrama de Casos de Uso - SabiApp

```mermaid
graph TD
    %% Actores
    Senior(("Usuario Sénior"))
    Tutor(("Tutor / Formador"))

    %% Subgraph del Sistema SabiApp
    subgraph SabiApp ["SabiApp"]
        UC01["UC01: Registrarse / Iniciar Sesión"]
        
        %% Módulos Sénior
        UC02["UC02: Practicar en Simuladores (Sandboxes)"]
        UC03["UC03: Realizar Talleres"]
        UC04["UC04: Consultar Ayuda Pedagógica"]

        %% Módulos Tutor
        UC05["UC05: Vincular Alumno Sénior"]
        UC06["UC06: Consultar Progreso"]
        UC07["UC07: Asignar Ejercicios o Módulos"]
    end

    %% Relaciones Usuario Sénior
    Senior --> UC01
    Senior --> UC02
    Senior --> UC03

    %% Relaciones Tutor
    Tutor --> UC01
    Tutor --> UC05
    Tutor --> UC06
    Tutor --> UC07

    %% Inclusiones (<<include>>)
    UC02 -. "<<include>>" .-> UC01
    UC03 -. "<<include>>" .-> UC01
    UC05 -. "<<include>>" .-> UC01
    UC06 -. "<<include>>" .-> UC01
    UC07 -. "<<include>>" .-> UC01

    UC02 -. "<<include>>" .-> UC04
    UC03 -. "<<include>>" .-> UC04

```

Prototipos de Interfaz de Usuario
Este es un prototipo de la pantalla del usuario senior, especificamente el apartado del banco 
┌────────────────────────────────────────────────────────┐
│ SABIAPP                                    [?] Ayuda   │
├────────────────────────────────────────────────────────┤
│                                                        │
│   [!] ENTORNO DE PRACTICA SEGURO                       │
│   (Sus cuentas y dinero real NO corren ningun riesgo)  │
│                                                        │
├────────────────────────────────────────────────────────┤
│                                                        │
│  PASO 1 DE 3: Elija a quien enviar el dinero           │
│                                                        │
│  ┌──────────────────────────────────────────────────┐  │
│  │  [Contacto] Maria (Hija)           612 345 678   │  │
│  └──────────────────────────────────────────────────┘  │
│  ┌──────────────────────────────────────────────────┐  │
│  │  [Contacto] Juan (Nieto)           699 887 766   │  │
│  └──────────────────────────────────────────────────┘  │
│  ┌──────────────────────────────────────────────────┐  │
│  │  [+] Escribir un numero nuevo                    │  │
│  └──────────────────────────────────────────────────┘  │
│                                                        │
├────────────────────────────────────────────────────────┤
│                                                        │
│  ┌────────────────────────┐  ┌──────────────────────┐  │
│  │  [<-] VOLVER AL MENU   │  │  CONTINUAR [->]      │  │
│  │  (Sin guardar)         │  │  (Paso siguiente)    │  │
│  └────────────────────────┘  └──────────────────────┘  │
│                                                        │
└────────────────────────────────────────────────────────┘

Este es un prototipo de la pantalla del usuario senior, especificamente el apartado del anti fraude. 

┌────────────────────────────────────────────────────────┐
│  SABIAPP - APRENDE A DETECTAR FRAUDES                  │
├────────────────────────────────────────────────────────┤
│                                                        │
│  [SMS] Ha recibido el siguiente mensaje en su movil:   │
│                                                        │
│  ┌──────────────────────────────────────────────────┐  │
│  │  De: +34 600 000 999                              │  │
│  │                                                  │  │
│  │  "CORREOS: Su paquete no se ha podido entregar    │  │
│  │   por faltar el n° de calle. Pague 1,89 EUR aqui:  │  │
│  │   http://correos-entrega-incidencia.com/pago"      │  │
│  └──────────────────────────────────────────────────┘  │
│                                                        │
│  ¿Que debe hacer con este mensaje?                     │
│                                                        │
│  ┌──────────────────────────────────────────────────┐  │
│  │  1. Pulsar el enlace para pagar los 1,89 EUR      │  │
│  └──────────────────────────────────────────────────┘  │
│  ┌──────────────────────────────────────────────────┐  │
│  │  2. Borrar el mensaje y NO pulsar en el enlace    │  │
│  └──────────────────────────────────────────────────┘  │
│                                                        │
│  [*] Pista: Mire atentamente la direccion web (URL)    │
│                                                        │
└────────────────────────────────────────────────────────┘

Este es un prototipo de la pantalla del usuario tutor.

┌────────────────────────────────────────────────────────────────────────┐
│  SABIAPP - PANEL DEL TUTOR                          [ Mi Cuenta (Tutor) ]│
├────────────────────────────────────────────────────────────────────────┤
│                                                                        │
│  Familiar supervisado: [ Carmen Mendoza (72 años) v ]   [ + Vincular ] │
│                                                                        │
│  ┌───────────────────────┐ ┌───────────────────────┐ ┌───────────────┐ │
│  │ Modulos Completados   │ │ Tasa de Aciertos      │ │ Dificultad    │ │
│  │      6 de 8           │ │        85%            │ │ Pantalla      │ │
│  └───────────────────────┘ └───────────────────────┘ └───────────────┘ │
│                                                                        │
│  Detalle de Rendimiento y Bloqueos Recientes:                          │
│  ┌───────────────────────────┬─────────────┬─────────────────────────┐ │
│  │ Modulo de Simulacion      │ Estado      │ Puntos de Atasco/Error  │ │
│  ├───────────────────────────┼─────────────┼─────────────────────────┤ │
│  │ Cita Medica (Salud)       │ Superado    │ Ninguno (Fluido)        │ │
│  │ Bizum Ficticio (Banca)    │ En progreso │ Duda al introducir PIN  │ │
│  │ Taller SMS (Ciberestafas) │ Superado    │ Requirio 2 intentos     │ │
│  └───────────────────────────┴─────────────┴─────────────────────────┘ │
│                                                                        │
│  Recomendaciones de la aplicacion:                                     │
│  "Carmen tiene dificultades para diferenciar el boton de 'Confirmar'   │
│   del boton de 'Cancelar' en operaciones bancarias. Se sugiere         │
│   reforzar esa leccion juntos."                                        │
│                                                                        │
└────────────────────────────────────────────────────────────────────────┘
