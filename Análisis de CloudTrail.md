Análisis de CloudTrail

1. Origen de la creación de la instancia EC2

Según el evento RunInstances de CloudTrail, la instancia EC2 fue creada por el servicio AWS Auto Scaling.

-Servicio que inició la solicitud: autoscaling.amazonaws.com
- Servicio de AWS que recibió la solicitud ec2.amazonaws.com
- Identidad utilizada: AWSServiceRoleForAutoScaling
- ID de la instancia: i-06e1716f46f968132
- Grupo de Auto Scaling: Examen-Modulo2-Paulalopez
- Región: us-east-1

El campo sourceIPAddress muestra autoscaling.amazonaws.com, lo que indica que la solicitud fue iniciada por el servicio Auto Scaling y no directamente desde la dirección IP del usuario.

2. Últimas cinco acciones del usuario IAM

Usuario IAM: PaulaAndreaLopezGomez

1. ListDiscoveredResources 26/10/2026, 21:56:42 — AWS Config.
2. DescribeConfigurationRecorderStatus 26/10/2026, 21:56:41 — AWS Config.
3. ListManagedNotificationEvents — 26/10/2026, 21:56:34 — AWS Notifications.
4. DescribeTrails — 26/10/2026, 21:56:23 — AWS CloudTrail.
5. LookupEvents — 26/10/2026, 21:56:23 — AWS CloudTrail.

Las cinco acciones mostradas no presentan errores registrados en los eventos consultados.
