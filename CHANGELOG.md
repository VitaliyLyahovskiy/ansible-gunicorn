## 1.3.0

- Add parameter `gunicorn_timeout` for configuring the timeout.

## 1.2.2

- Fix service suffix when using `systemd` to append `.service`.

## 1.2.1

- Fix threading through of `gunicorn_start_on` to `systemd` unit `WantedBy`.

## 1.2.0

- Add `systemd` Unit when `systemd` is the default OS service manager.

## 1.1.0

- Add `gunicorn_dynamic_workers` parameter to dynamically increase the number of workers with the number of CPUs.
- Add `gunicorn_cpu_coefficient` parameter to increase the amount of workers per CPU when `gunicorn_dynamic_workers` is `True`.

## 1.0.1

- Add support for setting `gunicorn_accesslog` and `gunicorn_errorlog` to `None`.

## 1.0.0

- Add `gunicorn_syslog` parameter to enable sending `stdout` and `stderr`
  output to syslog.
- Make access log and error log output to `stdout` and `stderr` so output
  routes to syslog.

## 0.1.0

- Initial release.
