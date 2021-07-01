targets += minecraft
project = $(notdir $(PWD))
port = 25565

ifeq ($(port),)
PORT=25565
else
PORT=$(port):25565
endif

attach=false
ifneq ($(attach),true)
up_opts += --detach
endif

volumes=false
ifeq ($(volumes),true)
down_opts += --volumes
endif

build:
	docker compose build $(targets)

run:
	PORT=$(PORT) \
	docker compose --project-name $(project) up $(up_opts)

clean:
	docker compose --project-name $(project) down $(down_opts)
