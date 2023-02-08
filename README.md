# e-commerce-backend
go mod init github.com/YOUR_GITHUB_USERNAME/golang-gorm-postgres

# docker
docker-compose.yml
docker-compose up -d
docker-compose down
docker exec -it postgres bash

# load env
go get github.com/spf13/viper

# connect to postgreSQL
go get -u gorm.io/gorm  
go get gorm.io/driver/postgres

# uuid ossp
psql -U admin golang-gorm
select * from pg_available_extensions;
CREATE EXTENSION IF NOT EXISTS "uuid-ossp";

# migration
