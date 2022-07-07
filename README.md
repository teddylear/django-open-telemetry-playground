# Django open telemetry playground

Sample Django app with open telemetry testing some concepts

## Running test server

```zsh
pipenv sync --dev
pipenv shell
cd demo_project
DJANGO_SETTINGS_MODULE=demo_project.settings opentelemetry-instrument python manage.py runserver --noreload
```

## Hitting test endpoint

`http://127.0.0.1:8000/helloWorld/`
