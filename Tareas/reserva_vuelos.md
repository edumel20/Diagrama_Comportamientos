# Tarea Reserva de Vuelos
___
### Descripción de la tarea
Crea un diagrama de casos de uso para un sistema de reservas de vuelos. Los actores pueden ser "Pasajero" y "Agente de Reservas". Algunos casos de uso podrían ser "Buscar Vuelo", "Reservar Vuelo", "Cancelar Reserva", etc.

![reserva_vuelos drawio](https://github.com/edumel20/Diagrama_Comportamientos/assets/145054591/b848b03c-8fb8-46be-960b-f09c5740131d)

___
### Actores

#### 1er Actor
|  Actor | Pasajero |
|---|---|
| Descripción  |Persona que busca y reserva vuelos.|
| Características  |Usuario registrado en el sistema. Busca información y realiza reservas.|
| Relaciones |Puede tener una relación similar con el Agente de Reservas al realizar operaciones de reserva.|
| Referencias |Buscar Vuelo, Reservar Vuelo, Cancelar Reserva.|
| Notas |Puede haber diferentes tipos de pasajeros, como pasajero frecuente.|
| Autor  | Eduardo Rabadán Melián |
|Fecha |23/01/2024 |


#### 2º Actor
|  Actor | Agente de Reservas |
|---|---|
| Descripción  |Personal encargado de asistir y gestionar reservas de vuelos.|
| Características  |Usuario registrado en el sistema con funciones adicionales. Gestiona reservas y genera informes.|
| Relaciones |Puede tener una relación similar con el Pasajero al realizar operaciones de reserva.|
| Referencias |Gestionar Reservas (Agente de Reservas), Generar Informe de Reservas (Agente de Reservas).|
| Notas |Puede haber diferentes roles de agentes, como agente de reservas junior o senior.|
| Autor  | Eduardo Rabadán Melián |
|Fecha |23/01/2024 |

___
### Casos de Uso

#### 1. Buscar Vuelo:

|  Caso de Uso	CU | Buscar Vuelo  |
|---|---|
| Fuentes  | reserva de vuelos |
| Actor  |  Pasajero. |
| Descripción |El Pasajero busca vuelos por destino, fecha y preferencias.|
| Flujo básico |1-> El Pasajero inicia sesión en el sistema. 2-> El Pasajero busca vuelos por destino, fecha y preferencias. 3-> El Sistema muestra una lista de vuelos disponibles.|
| Pre-condiciones | El Pasajero está autenticado en el sistema.|  
| Post-condiciones  | El Sistema muestra los vuelos disponibles.|  
|  Requerimientos | Ninguno en particular. |
|  Notas | Puede haber opciones avanzadas de búsqueda.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 2. Reservar Vuelo:

|  Caso de Uso	CU | Reservar Vuelo  |
|---|---|
| Fuentes  | reserva de vuelos |
| Actor  |  Pasajero, Agente de Reservas. |
| Descripción |El Pasajero reserva un vuelo seleccionado. El Sistema solicita confirmación y genera una confirmación de reserva.|
| Flujo básico |1-> El Pasajero inicia sesión en el sistema. 2-> El Pasajero busca y selecciona un vuelo. 3-> El Sistema solicita confirmación de reserva. 4-> El Pasajero confirma la reserva. 5-> El Sistema genera una confirmación de reserva.|
| Pre-condiciones |El Pasajero está autenticado en el sistema y hay vuelos disponibles.|  
| Post-condiciones  |El Sistema confirma y registra la reserva.|  
|  Requerimientos |El vuelo seleccionado debe estar disponible.|
|  Notas |El Agente de Reservas puede asistir en el proceso.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 3. Cancelar Reserva:

|  Caso de Uso	CU | Cancelar Reserva  |
|---|---|
| Fuentes  | reserva de vuelos |
| Actor  |  Pasajero, Agente de Reservas. |
| Descripción |El Pasajero cancela una reserva existente. El Sistema solicita confirmación y actualiza el estado de la reserva.|
| Flujo básico |1-> El Pasajero inicia sesión en el sistema. 2-> El Pasajero accede a su historial de reservas. 3-> El Pasajero selecciona una reserva para cancelar. 4-> El Sistema solicita confirmación de cancelación. 5-> El Pasajero confirma la cancelación. 6-> El Sistema actualiza el estado de la reserva.|
| Pre-condiciones |El Pasajero está autenticado en el sistema y tiene reservas existentes.|  
| Post-condiciones  |La reserva seleccionada se cancela y el estado se actualiza.|  
|  Requerimientos |El Pasajero debe tener reservas existentes.|
|  Notas |El Agente de Reservas puede asistir en el proceso.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 4. Gestionar Reserva:

|  Caso de Uso	CU | Gestionar Reserva  |
|---|---|
| Fuentes  | reserva de vuelos |
| Actor  |  Agente de Reservas. |
| Descripción |El Agente de Reservas gestiona las reservas, pudiendo ver, modificar o cancelar reservas según sea necesario.|
| Flujo básico |1-> El Agente de Reservas inicia sesión en el sistema. 2-> El Agente de Reservas accede a la lista de reservas. 3-> El Agente de Reservas puede ver, modificar o cancelar reservas.|
| Pre-condiciones |El Agente de Reservas está autenticado en el sistema.|  
| Post-condiciones  |La información de las reservas se actualiza según las acciones del Agente de Reservas.|  
|  Requerimientos |Ninguno en particular.|
|  Notas |Puede incluir detalles adicionales sobre las acciones permitidas.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 5. Generar Informe de Reservas:

|  Caso de Uso	CU | Generar Informe de Reservas  |
|---|---|
| Fuentes  | reserva de vuelos |
| Actor  |  Agente de Reservas. |
| Descripción |El Agente de Reservas genera un informe con estadísticas y detalles de las reservas realizadas.|
| Flujo básico |1-> El Agente de Reservas inicia sesión en el sistema. 2-> El Agente de Reservas selecciona la opción de generar un informe. 3-> El Sistema genera un informe con estadísticas y detalles de las reservas.|
| Pre-condiciones |El Agente de Reservas está autenticado en el sistema.|  
| Post-condiciones  |Se genera un informe con información sobre las reservas.|  
|  Requerimientos |Ninguno en particular.|
|  Notas |Puede incluir detalles adicionales sobre el formato del informe.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |
