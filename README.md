# ms-eureka-server

Servidor de descubrimiento Eureka para Servillantas RV.

Arranca después de Config Server. Su archivo local contiene únicamente el nombre de aplicación y la dirección de Config Server; puerto, hostname y comportamiento de Eureka se obtienen centralmente desde `ms-eureka-server.yml`.

- Puerto por defecto: `8761`
- Dashboard: `/`
- Health: `/actuator/health`
- Registro: `/eureka/apps`
