Diagrama de Casos de Uso - SabiApp

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
