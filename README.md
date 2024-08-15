# Products Microservice

## Dev
1. Clonar el repositorio
2. Instalar dependencias
3. Crear un archivo `.env` basado en el `env.template`
4. Levantar el servidor de NATS 
```
docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```
5. Ejecutar migracion de prisma `npx prisma migrate dev`
6. Tener levantados los microservicios que se van a consumir
7. Levantar proyecto con `npm run start:dev`