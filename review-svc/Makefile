# version 1
build-1.0.0:
	docker build -t rahadiangg/demo-istio:review-svc-1.0.0 -f Dockerfile-1.0.0 .

run-1.0.0:
	docker run --rm -p 8001:8000 rahadiangg/demo-istio:review-svc-1.0.0

# version 2
build-2.0.0:
	docker build -t rahadiangg/demo-istio:review-svc-2.0.0 -f Dockerfile-2.0.0 .

run-2.0.0:
	docker run --rm -p 8001:8000 rahadiangg/demo-istio:review-svc-2.0.0

# version 3
build-3.0.0:
	docker build -t rahadiangg/demo-istio:review-svc-3.0.0 -f Dockerfile-3.0.0 .

run-3.0.0:
	docker run --rm -p 8001:8000 rahadiangg/demo-istio:review-svc-3.0.0

## build all and push to registry
build-and-push-all:
	docker buildx build -t rahadiangg/demo-istio:review-svc-1.0.0 -f Dockerfile-1.0.0 --platform=linux/arm64,linux/amd64 --push .
	docker buildx build -t rahadiangg/demo-istio:review-svc-2.0.0 -f Dockerfile-2.0.0 --platform=linux/arm64,linux/amd64 --push .
	docker buildx build -t rahadiangg/demo-istio:review-svc-3.0.0 -f Dockerfile-3.0.0 --platform=linux/arm64,linux/amd64 --push .