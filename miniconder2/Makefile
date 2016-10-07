docker_registry = liebeck
name = miniconder2
tag = 0.0.1

.PHONY: build

all: build

build:
	docker build -t $(docker_registry)/$(name) .

run:
	docker run -it $(docker_registry)/$(name) bash -l

push:
	docker push $(docker_registry)/$(name)
