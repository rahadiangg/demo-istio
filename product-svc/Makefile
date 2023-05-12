build:
	docker build -t rahadiangg/demo-istio:product-svc-1.0.0 .

build-and-push-all:
	docker buildx build -t rahadiangg/demo-istio:product-svc-1.0.0 --platform=linux/arm64,linux/amd64 --push .

run:
	docker run --rm -p 8000:8000 rahadiangg/demo-istio:product-svc-1.0.0