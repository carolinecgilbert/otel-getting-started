# otel-getting-started

## Getting Started with OpenTelemetry
[https://opentelemetry.io/docs/languages/python/getting-started/](https://opentelemetry.io/docs/languages/python/getting-started/)

## Installation
`python3 -m venv venv`

`source ./venv/bin/activate`

## Run the Instrumented App
`export OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED=true
opentelemetry-instrument \
    --traces_exporter console \
    --metrics_exporter console \
    --logs_exporter console \
    --service_name dice-server \
    flask run -p 8080`
