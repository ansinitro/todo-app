# REST API for creating TODO lists in Go #
<hr>

### This project was created based on the <a href="https://www.youtube.com/playlist?list=PLbTTxxr-hMmyFAvyn7DeOgNRN8BQdjFm8">YouTube tutorial</a> ###
<hr>

#### The following concepts are covered in the course: ####
- Developing Web Applications in Go, following REST API design principles.
- Working with the gin-gonic/gin framework.
- Applying Clean Architecture principles in building application structure. Dependency injection technique.
- Working with Postgres database. Generation of migration files.
- Application configuration using the spf13/viper library. Handling environment variables.
- Database interaction using the sqlx library.
- User registration and authentication. Working with JWT. Middleware.
- Writing SQL queries.
- Graceful Shutdown.
<hr>

#### Quick Start ####

```bash
    git clone "https://github.com/ansinitro/todo-app" 
    cd todo-app
    go mod download
```
create `.env` file based on `.env.example` file or just execute `echo DB_PASSWORD=<your_password> > .env`
```bash
    migrate -path ./schema -database 'postgres://postgres:<your_password>@0.0.0.0:5432/postgres?sslmode=disable' up
    go run cmd/main.go
```