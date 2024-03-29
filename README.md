﻿# pkk-backend-v2
go mod init github.com/YOUR_GITHUB_USERNAME/golang-gorm-postgres
docker-compose.yml
app.env
.gitignore
# Docker
docker-compose up -d
docker-compose down

go get github.com/spf13/viper
initializers/loadEnv.go
go get -u gorm.io/gorm  
go get gorm.io/driver/postgres
initializers/connectDB.go
models/user.model.go
docker exec -it postgres bash

# migrate
psql -U admin golang-gorm
select * from pg_available_extensions;
CREATE EXTENSION IF NOT EXISTS "uuid-ossp";
migrate/migrate.go
# air
go get github.com/gin-gonic/gin
go install github.com/cosmtrek/air@latest
main.go
air

# binary will be $(go env GOPATH)/bin/air
curl -sSfL https://raw.githubusercontent.com/cosmtrek/air/master/install.sh | sh -s -- -b $(go env GOPATH)/bin

# or install it into ./bin/
curl -sSfL https://raw.githubusercontent.com/cosmtrek/air/master/install.sh | sh -s

air -v

go install github.com/cosmtrek/air@latest

run
air -c .air.toml

air init
