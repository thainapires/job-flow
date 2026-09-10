
  cd api
  cp .env.example .env
  make up
  make migrate

  Testes:

  cd api
  make test

  Formatter/lint:

  cd api
  make lint
  make format