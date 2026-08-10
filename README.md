# test-cd

## Spring Boot SSR sample

A simple Spring Boot app is available at:

`/home/runner/work/test-cd/test-cd/spring-boot-ssr`

Endpoints:
- `/health` → returns `OK`
- `/` → renders SSR HTML page with message: `Hello perfectly done deployment`

Run locally:

```bash
cd /home/runner/work/test-cd/test-cd/spring-boot-ssr
mvn spring-boot:run
```

Run with Docker:

```bash
cd /home/runner/work/test-cd/test-cd/spring-boot-ssr
docker build -t spring-boot-ssr .
docker run --rm -p 8080:8080 spring-boot-ssr
```
