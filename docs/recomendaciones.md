# Recomendaciones de mejora

Aportación de **Justin Emiliano Rodríguez Franco (`justin12f`)** como
colaborador externo del proyecto Organizador Personal (repositorio de
`santsss01`). A continuación se listan sugerencias para fortalecer la estructura
y la documentación del proyecto.

## 1. Definir un modelo de datos para tareas y notas

Antes de programar, conviene describir en `docs/` los campos de una tarea (id,
título, descripción, fecha límite, estado, etiquetas) y de una nota (id, texto,
tarea asociada, fecha). Así la implementación parte de una estructura clara y
estable en lugar de improvisarse.

## 2. Agregar un archivo `.env.example`

El proyecto incluye `python-dotenv` y `.env` está en `.gitignore`, pero no hay
una plantilla que indique qué variables espera la aplicación. Se recomienda
versionar un `.env.example` con las claves esperadas y sin valores reales:

```
API_URL=
API_TOKEN=
```

## 3. Completar los pasos de instalación con la evidencia de ejecución

En `README.md`, la sección de instalación ya está bien; conviene añadir la
salida esperada al ejecutar el proyecto, como prueba mínima de que el entorno
quedó bien configurado:

```
$ python src/main.py
Organizador Personal
```

## 4. Separar la lógica futura en módulos dentro de `src/`

En lugar de concentrar todo en `main.py`, prever desde ahora una organización
por responsabilidades (por ejemplo `tareas.py`, `notas.py`,
`almacenamiento.py`), de modo que el proyecto pueda crecer sin volverse difícil
de mantener.

## 5. Agregar pruebas automatizadas con `pytest`

El proyecto no cuenta con pruebas. Se recomienda crear una carpeta `tests/` con
un test mínimo que verifique la salida de `src/main.py` y registrar `pytest` en
`requirements.txt`, para tener una base sobre la cual añadir pruebas conforme
avance la implementación.
