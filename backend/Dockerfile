FROM golang:1.21

WORKDIR /app

# 安装热重载工具
RUN go install github.com/air-verse/air@latest

# 复制项目文件
COPY go.mod go.sum ./
RUN go mod download

COPY . .
