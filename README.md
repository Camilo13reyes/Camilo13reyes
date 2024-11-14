@startuml
left to right direction

actor Usuario as User
actor "Personal de Parqueadero" as Staff
actor "Sistema de Parqueadero" as System

rectangle "Parqueo Seguro" {
    User --> (Registrar entrada y salida) : "Acceso rápido"
    User --> (Consultar disponibilidad de espacios) : "Consulta en tiempo real"
    User --> (Realizar pagos) : "Opciones múltiples"
    User --> (Recibir notificaciones) : "Alertas automáticas"
    User --> (Consultar promociones y descuentos) : "Beneficios adicionales"

    Staff --> (Atención al cliente) : "Soporte a usuarios"
    Staff --> (Gestionar seguridad) : "Monitoreo y asistencia"

    System --> (Monitoreo de espacios automatizado) : "Disponibilidad en tiempo real"
    System --> (Reconocimiento de matrículas) : "Entrada y salida automáticas"
}

@enduml
