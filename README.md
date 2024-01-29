<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Execute on development

1. Clone repositorie
2. Execute

```
npm install
```

3. Install Nest CLI
```
npm i -g @nestjs/cli
```

4. Start db
```
docker compose up -d
```

5. Clone the __.env.template__ and rename it to __.env__

6. Fill the enviroment variables in the __.env__ file

7. Run app in development mode: 

```
npm run start:dev
```

8. Rebuild database with the seed
```
http://localhost:3000/seed
```

# Production Build

1. Create ```.env.prod``` file.
2. Fill enviroment variables.
3. Create the new image:

```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```

## Used Stack
* MongoDB
* Nest