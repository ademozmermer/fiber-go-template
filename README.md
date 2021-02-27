# Fiber backend template for [Create Go App CLI](https://github.com/create-go-app/cli)

<img src="https://img.shields.io/badge/Go-1.16+-00ADD8?style=for-the-badge&logo=go" alt="go version" />&nbsp;<a href="https://gocover.io/github.com/create-go-app/fiber-go-template/pkg/apiserver" target="_blank"><img src="https://img.shields.io/badge/Go_Cover-87%25-success?style=for-the-badge&logo=none" alt="go cover" /></a>&nbsp;<a href="https://goreportcard.com/report/github.com/create-go-app/fiber-go-template" target="_blank"><img src="https://img.shields.io/badge/Go_report-A+-success?style=for-the-badge&logo=none" alt="go report" /></a>&nbsp;<img src="https://img.shields.io/badge/license-mit-red?style=for-the-badge&logo=none" alt="license" />

[Fiber](https://gofiber.io/) is an Express.js inspired web framework build on top of Fasthttp, the fastest HTTP engine for Go. Designed to ease things up for **fast** development with **zero memory allocation** and **performance** in mind.

## ⚡️ Quick start

1. Create a new project:

```bash
cgapp create
```

2. Run project by this command:

```bash
make run
```

## ✅ Used packages

- [gofiber/fiber](https://github.com/gofiber/fiber) `v2.5.0`
- [joho/godotenv](https://github.com/) `v1.3.0`
- [stretchr/testify](https://github.com/stretchr/testify) `v1.7.0`

## 🗄 Template structure

```bash
.
├── .dockerignore
├── .editorconfig
├── .gitignore
├── .env.example
├── Dockerfile
├── Makefile
├── go.mod
├── go.sum
├── main.go
├── static
│   └── index.html
└── pkg
    └── apiserver
        ├── config.go
        ├── config_test.go
        ├── error_checker.go
        ├── error_checker_test.go
        ├── new_server.go
        ├── new_server_test.go
        ├── routes.go
        ├── utils.go
        └── utils_test.go

3 directories, 17 files
```

## ⚙️ Configuration

```yaml
# ./configs/apiserver.yml

# Server config
server:
  host: 0.0.0.0
  port: 5000

# Database config
database:
  host: 127.0.0.1
  port: 5432
  username: postgres
  password: 1234

# Static files config
static:
  prefix: /
  path: ./static
```

## ⚠️ License

MIT &copy; [Vic Shóstak](https://github.com/koddr) & [True web artisans](https://1wa.co/).
