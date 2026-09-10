# Organizador Personal

## Objetivo

Preparar la estructura inicial de una aplicación que, en el futuro, podría
administrar tareas y notas personales. En esta práctica el foco no es la
programación, sino el uso correcto de Visual Studio Code, el entorno virtual,
las dependencias, Git y GitHub.

## Tecnologías utilizadas

- Python 3.12
- Entorno virtual `venv`
- Git y GitHub
- Visual Studio Code
- Bibliotecas: `requests`, `python-dotenv`

## Pasos de instalación

```bash
# 1. Clonar el repositorio
git clone <URL_DEL_REPOSITORIO>
cd organizador-personal-integradora-santi

# 2. Crear y activar el entorno virtual
python -m venv .venv
source .venv/bin/activate        # macOS / Linux
# .venv\Scripts\activate         # Windows

# 3. Instalar las dependencias
pip install -r requirements.txt

# 4. Ejecutar
python src/main.py
```

## Dependencias

Registradas en `requirements.txt` mediante `pip freeze`:

- `requests`
- `python-dotenv`
- (dependencias transitivas: `certifi`, `charset-normalizer`, `idna`, `urllib3`)

## Autor

santsss01 — Desarrollo de Aplicaciones y Servicios Virtuales, Ing. Alejandro
Montes, Universidad Iberoamericana León.

## Estado

Proyecto en etapa inicial. Actualmente se encuentra lista la estructura base,
el entorno virtual, la gestión de dependencias y el control de versiones. Las
funcionalidades descritas en `docs/funcionalidades.md` aún no están
implementadas.

## Colaboración

Este proyecto se desarrolló en parejas como parte de la práctica integradora de
Git y GitHub.

- El repositorio original pertenece a **santsss01**.
- **justin12f** participó como colaborador externo: creó un *fork*, trabajó en la
  rama `mejora-documentacion` y propuso cambios mediante un *Pull Request*
  (`docs/recomendaciones.md` y esta sección).
- La propietaria revisó el Pull Request, lo aprobó y realizó el *merge* hacia
  `main`.

Flujo utilizado: fork → clone → branch → commit → push → Pull Request → review →
merge → pull.
