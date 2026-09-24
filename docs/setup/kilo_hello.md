# kilo_hello

готов

1. Учебный сервис предварительной оценки заявки на заём под ПТС: принимает заявку (VIN, год, пробег, стоимость, сумма, срок), считает LTV и возвращает решение `approve` / `review` / `reject`.
2. Makefile: `make up`, `down`, `ps`, `logs`, `install`, `test` (PHPUnit), `lint` (php -l), `seed`, `help`; отдельных команд запуска/проверки в docker-compose.yml не нашёл — там только сервисы `backend` и `db` (у db — healthcheck).
3. Решение approve / review / reject считается в `backend/src/Domain/` — `DecisionEngine.php` по порогам LTV.

модель: training-2026-09-glm-5.3
