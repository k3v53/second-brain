---
title: 
aliases: 
tags:
  - Español
  - k8s
draft: false
status: Investigating
---
> [!todo] Pendiente
> Todavía estoy escribiendo sobre el tópico mientras estudio, te agradecería si me aportas contribuciones constructivas para mejorar la información y permitir que exista más material en español de kubernetes en internet.

Kubernetes (también conocido como K8s) es una plataforma open source para la [[Orquestador de Contenedores|orquestación de contenedores]] y microservicios. Fue originalmente diseñado por Google y ahora está mantenido por una comunidad global de contribuyentes.
^desc

Existen variantes que integran fundamentalmente el mismo concepto de kubernetes pero de diferentes formas como minikube, k3s, etc. La mayoría de estas soluciones tienen paridad de features con el kubernetes original pero modifican el funcionamiento para hacerlo más liviano, más completo, mejor integración con windows, etc.
### Características principales

- Orquestación de contenedores: Automatiza el despliegue, escalado y manejo de aplicaciones en contenedores.
- Portabilidad: Permite ejecutar aplicaciones en diferentes entornos, desde la nube hasta el data center.
- Escalabilidad: Facilita el aumento o disminución de recursos según sea necesario.
- Autohealing: Revisa constantemente el estado de los contenedores y los restaura automáticamente si fallan.

### Componentes clave

- Control Plane: Gestiona el estado del clúster y coordina las acciones.
- Node: Los servidores donde se ejecutan los contenedores.
- Pods: La menor unidad de despliegue y ejecución en Kubernetes.
- Services: Exponen los pods internos para que puedan ser accesados externamente.

### Funciones de Kubernetes

Kubernetes se encarga de:

- Distribuir contenedores entre los nodos del clúster.
- Garantizar que el número correcto de réplicas estén ejecutándose.
- Manejar la actualización de aplicaciones de forma suave.
- Proporcionar herramientas para monitoreo y observabilidad.

### Ecosistema

Kubernetes tiene un ecosistema extenso con herramientas adicionales como:

- Helm: Para gestión de paquetes de aplicaciones.
- Istio: Para servicio y monitoreo.
- Prometheus y Grafana: Para monitoreo y visualización de métricas.

> [!todo] Pendiente: Hay más herramientas, iré listando mientras las vaya utilizando

### Uso y adopción

Kubernetes es ampliamente utilizado por empresas como Google, Microsoft, Amazon, Apple, Meta y muchas otras. Es uno de los sistemas de software más utilizados en el mundo.

En resumen, Kubernetes es una plataforma poderosa para gestionar aplicaciones contenedorizadas de forma eficiente y escalable, permitiendo a las organizaciones aprovechar los beneficios de la nube y la microservicios.
## Cargas de Trabajo (Workloads)
Un workload es una aplicación o servicio que se ejecuta en Kubernetes. Es un nivel más alto de abstracción que agrupa uno o más contenedores y define cómo deben ser empaquetados, desplegados, gestionados y escalados.
Cuando se crea un workload, define un estado deseado (por ejemplo, el número de réplicas de pods que deben estar ejecutándose). Kubernetes monitorea el estado actual del clúster y compara con el deseado. Si no coinciden, el controlador toma acción para acercar el estado real al deseado.
Los workloads manejan operaciones como escalado, actualizaciones sucesivas y auto-reparación de fallos.
## Tipos de Workloads
- Deployment: Para mantener un conjunto estable de pods.
- ReplicaSet: Similar a Deployments pero más básico.
- StatefulSet: Para aplicaciones con estado definido.
- DaemonSet: Para ejecutar un pod en cada nodo del clúster.
- Job: Para tareas que deben completarse.
- CronJob: Para tareas que deben completarse de manera cronológica.


