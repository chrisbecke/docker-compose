targets += minecraft
project = $(notdir $(PWD))
port = 25565:

build:
	docker compose build $(targets)

up:
	PORT=$(port) \
	docker compose --project-name $(project) up --detach