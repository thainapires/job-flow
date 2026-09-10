COMPOSE=docker compose

.PHONY: up down install migrate test lint format shell

up:
	$(COMPOSE) up -d --build

down:
	$(COMPOSE) down

install:
	$(COMPOSE) run --rm app composer install

migrate:
	$(COMPOSE) run --rm app php artisan migrate

test:
	$(COMPOSE) run --rm app composer test

lint:
	$(COMPOSE) run --rm app composer lint

format:
	$(COMPOSE) run --rm app composer format

shell:
	$(COMPOSE) run --rm app sh
