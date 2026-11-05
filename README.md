# MS Eureka Server

Registro y descubrimiento de los microservicios de Servillantas.

## Responsabilidades

- Recibe el registro y los latidos de cada instancia.
- Permite que el API Gateway y los clientes usen nombres lógicos en vez de hosts fijos.
- Expone el panel de Eureka y el endpoint `/eureka/`.
- No se registra a sí mismo ni descarga otro registro.

El puerto predeterminado es `8761`; la configuración proviene de Config Server (`ms-eureka-server.yml`). En producción revise `EUREKA_SELF_PRESERVATION` antes de desactivarlo.

## Ejecución

Inicie primero Config Server y después Eureka:

```bash
./mvnw test
./mvnw spring-boot:run
```
