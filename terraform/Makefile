include version.env

.PHONY: help
help:
	@echo choose target

build:
	docker build --build-arg TERRAFORM_VERSION=$(VERSION) -t $(IMAGE):$(VERSION) .

push:
	docker push $(IMAGE):$(VERSION)
