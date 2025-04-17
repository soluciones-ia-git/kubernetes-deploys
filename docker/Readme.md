# Instalación

## App alerts

### Pasos previos

1. Copiar el `.env.example` y nombrarlo `.env`
2. Ajustar las variables de entorno

### Levantar el backend

```
docker-compose -f docker/app-alerts/docker-compose.back.yaml up -d
```

### Levantar el frontend

```
docker-compose -f docker/app-alerts/docker-compose.front.yaml up -d --build    
```

## App alerts revisión

> Levantar primero el backend principal, ya que es el que crea la red que compartira con la app de revisíon

### Pasos previos

1. Copiar el `.env.example` y nombrarlo `.env`
2. Ajustar las variables de entorno

### Levantar el backend

```
docker-compose -f docker/app-alerts-review/docker-compose.back.yaml up -d
```

### Levantar el frontend

```
docker-compose -f docker/app-alerts-review/docker-compose.front.yaml up -d --build    
```