.PHONY: init
# init
init:
	go install github.com/go-delve/delve/cmd/dlv@latest
	go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
	go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest
	go install github.com/go-kratos/kratos/cmd/kratos/v2@latest
	go install github.com/go-kratos/kratos/cmd/protoc-gen-go-http/v2@latest
	go install github.com/google/gnostic/cmd/protoc-gen-openapi@latest
	go install github.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2@latest
	go install github.com/go-kratos/kratos/cmd/protoc-gen-go-errors/v2@latest
	go install github.com/envoyproxy/protoc-gen-validate@latest
	go install github.com/google/wire/cmd/wire@v0.5.0
	
# docker login harbor-st.2345.cn                              登陆harbor
# docker buildx create --name multi-platform-builder --use    创建docker driver并使用
# docker buildx inspect --bootstrap                           拉取镜像moby/buildkit:buildx-stable-1
#.PHONY: build
#build:
#	docker buildx build --platform linux/amd64,linux/arm64 -f Dockerfile -t harbor-st.2345.cn/server/devcontainer-go-kratos:1.22.3 . --push
