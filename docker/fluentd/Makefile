USER=kkohtaka
PRODUCT=fluentd

IMAGE_NAME=$(USER)/$(PRODUCT)

.PHONY: build push

default: build
all: build push

build:
	docker build -t $(IMAGE_NAME) .

push: build
	docker push $(IMAGE_NAME)
