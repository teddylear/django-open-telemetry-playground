# Django open telemetry playground

Sample Django app with open telemetry testing some concepts

## Running test server

```zsh
pipenv sync --dev
pipenv shell
cd demo_project
DJANGO_SETTINGS_MODULE=demo_project.settings python manage.py runserver --noreload
```

## Hitting test endpoint

`http://127.0.0.1:8000/helloWorld/`

## Docs
- [Open Telemetry Django docs](https://opentelemetry-python.readthedocs.io/en/stable/examples/django/README.html)
- [Open Telemetry Django lib middleware code](https://github.com/open-telemetry/opentelemetry-python-contrib/blob/ee4083982f5919e1366de62b9cf4dac28cc8a314/instrumentation/opentelemetry-instrumentation-django/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py)

## TODO
- Add endpoints with values passed in
- Add parameters that are passed in to be always logged for context
