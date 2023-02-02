# pkk-backend-v2

# Docker
docker-compose up -d
docker-compose down
docker exec -it postgres bash

# migrate
psql -U admin golang-gorm
select * from pg_available_extensions;
CREATE EXTENSION IF NOT EXISTS "uuid-ossp";
migrate/migrate.go
# air

# binary will be $(go env GOPATH)/bin/air
curl -sSfL https://raw.githubusercontent.com/cosmtrek/air/master/install.sh | sh -s -- -b $(go env GOPATH)/bin

# or install it into ./bin/
curl -sSfL https://raw.githubusercontent.com/cosmtrek/air/master/install.sh | sh -s

air -v

go install github.com/cosmtrek/air@latest

run
air -c .air.toml

air init
