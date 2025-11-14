# iot-realtime-monitoring-kafka
Claro, aquí tienes una versión más limpia y profesional de la descripción para tu repositorio en GitHub, sin emojis ni divisores:

---

# Sistema de Monitoreo IoT en Tiempo Real con Apache Kafka, InfluxDB y Grafana

Este repositorio contiene la implementación de un sistema distribuido para monitoreo de sensores IoT en tiempo real, utilizando un pipeline de datos basado en Apache Kafka, almacenamiento en InfluxDB y visualización con Grafana.  

El proyecto está dockerizado para facilitar la instalación y despliegue, e incluye productores y consumidores en Python que simulan dispositivos enviando métricas de temperatura y humedad.

## Características principales
- Transmisión de eventos IoT en tiempo real con Kafka  
- Almacenamiento eficiente de métricas en InfluxDB  
- Dashboards dinámicos e interactivos en Grafana  
- Escalabilidad horizontal mediante múltiples consumidores  
- Entorno reproducible con Docker Compose  

## Tecnologías utilizadas
- Apache Kafka  
- Python (productores y consumidores)  
- InfluxDB  
- Grafana  
- Docker Compose  

## Estructura del proyecto
```
iot-kafka/
│── docker-compose.yml
│── producer/
│   ├── requirements.txt
│   └── producer.py
│── consumer/
│   ├── requirements.txt
│   └── consumer.py
```

## Ejecución
1. Clonar el repositorio:  
   ```bash
   git clone https://github.com/tuusuario/iot-realtime-monitoring-kafka.git
   cd iot-realtime-monitoring-kafka
   ```
2. Levantar los servicios:  
   ```bash
   docker compose up -d
   ```
3. Ejecutar el productor:  
   ```bash
   python3 producer/producer.py
   ```
4. Ejecutar el consumidor:  
   ```bash
   python3 consumer/consumer.py
   ```
5. Acceder a las interfaces:  
   - InfluxDB → http://localhost:8086  
   - Grafana → http://localhost:3000  

## Ejemplo de visualización
Los datos de temperatura y humedad se muestran en dashboards de Grafana en tiempo real, permitiendo validar el funcionamiento del sistema y analizar métricas históricas.
