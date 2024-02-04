# Tarea Sistema de Biblioteca
___
### Descripción de la tarea
Desarrolla un diagrama de casos de uso para un sistema de biblioteca. Los actores pueden ser "Usuario" y "Bibliotecario". Algunos casos de uso podrían ser "Prestar Libro", "Devolver Libro", "Buscar Libro", etc.

![sistema_biblioteca drawio](https://github.com/edumel20/Diagrama_Comportamientos/assets/145054591/6086cb22-9d12-41f4-a297-59cc5a2fc8c6)

___
### Actores



#### 1er Actor
|  Actor | Usuario |
|---|---|
| Descripción  |Individuo que utiliza el sistema de biblioteca para buscar, prestar y devolver libros.|
| Características  | Usuario registrado, busca información, realiza préstamos y devoluciones.|
| Relaciones | Puede tener una relación similar con el Bibliotecario al realizar operaciones como préstamos y devoluciones.|
| Referencias | Buscar Libro, Prestar Libro, Devolver Libro, Ver Información, Ver Historial.|
| Notas | Puede tener diferentes roles como estudiante, profesor, etc.|
| Autor  | Eduardo Rabadán Melián |
|Fecha |23/01/2024 |



#### 2º Actor
|  Actor | Bibliotecario |
|---|---|
| Descripción  | Personal de la biblioteca encargado de gestionar el inventario, realizar préstamos y devoluciones.|
| Características  | Acceso a funciones administrativas, gestión de inventario, confirmación de préstamos.|
| Relaciones | Puede tener una relación similar con el Usuario al realizar operaciones como préstamos y devoluciones.|
| Referencias | Prestar Libro, Devolver Libro, Gestionar Inventario.|
| Notas | Puede tener diferentes roles, como bibliotecario junior o senior.|
| Autor  | Eduardo Rabadán Melián |
|Fecha |23/01/2024 |

___
### Casos de Uso

#### 1. Buscar Libro:

|  Caso de Uso	CU | Buscar Libro  |
|---|---|
| Fuentes  | gestión de biblioteca |
| Actor  |  Usuario |
| Descripción | El usuario busca libros por título, autor o categoría.|
| Flujo básico | 1-> El usuario inicia sesión en el sistema. 2-> El usuario busca libros por título, autor o categoría.|
| Pre-condiciones | El usuario está autenticado en el sistema.|  
| Post-condiciones  | El sistema muestra los resultados de la búsqueda.|  
|  Requerimientos | Ninguno en particular. |
|  Notas | Ninguna. |
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 2. Prestar Libro:

|  Caso de Uso	CU | Prestar Libro  |
|---|---|
| Fuentes  | gestión de biblioteca |
| Actor  |  Usuario, Bibliotecario |
| Descripción | El usuario selecciona un libro para prestar. El sistema verifica la disponibilidad, solicita la confirmación al bibliotecario, el bibliotecario confirma el préstamo, y el sistema registra el préstamo y actualiza la disponibilidad del libro.|
| Flujo básico | 1-> El usuario inicia sesión en el sistema. 2-> El usuario busca y selecciona un libro disponible. 3-> El sistema verifica la disponibilidad del libro. 4-> El sistema solicita la confirmación al bibliotecario. 5-> El bibliotecario confirma el préstamo. 6-> El sistema registra el préstamo y actualiza la disponibilidad del libro. |
| Pre-condiciones | El usuario está autenticado en el sistema.|  
| Post-condiciones  | El libro queda prestado y disponible en el historial del usuario.|  
|  Requerimientos | El libro debe estar disponible en el inventario.|
|  Notas | Es posible agregar funcionalidades adicionales como recordatorios de devolución.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 3. Devolver Libro:

|  Caso de Uso	CU | Devolver Libro  |
|---|---|
| Fuentes  | gestión de biblioteca |
| Actor  |  Usuario, Bibliotecario |
| Descripción | El usuario devuelve un libro al sistema. El sistema registra la devolución y actualiza la disponibilidad del libro, generando un recibo.|
| Flujo básico | 1-> El usuario inicia sesión en el sistema. 2-> El usuario selecciona la opción de devolver un libro prestado. 3-> El sistema registra la devolución y actualiza la disponibilidad del libro. 4-> El sistema genera un recibo de devolución.|
| Pre-condiciones | El usuario está autenticado en el sistema y tiene libros prestados.|  
| Post-condiciones  | El libro queda disponible en el inventario y se genera un recibo de devolución.|  
|  Requerimientos | El usuario debe tener libros prestados. |
|  Notas | El recibo puede incluir detalles como la fecha y hora de devolución.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 4. Ver Información:

|  Caso de Uso	CU | Ver Información  |
|---|---|
| Fuentes  | gestión de biblioteca |
| Actor  |  Usuario. |
| Descripción | El usuario selecciona un libro y visualiza información detallada, como autor, año de publicación, etc.|
| Flujo básico | 1-> El usuario inicia sesión en el sistema. 2-> El usuario busca y selecciona un libro. 3-> El sistema muestra la información detallada del libro.|
| Pre-condiciones | El usuario está autenticado y ha buscado el libro.|  
| Post-condiciones  | El usuario ha visualizado la información detallada del libro.|  
|  Requerimientos | El libro debe existir en el inventario |
|  Notas | Puede incluir detalles adicionales sobre la información que se mostrará.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 5. Ver Historial:

|  Caso de Uso	CU | Ver Historial  |
|---|---|
| Fuentes  | gestión de biblioteca |
| Actor  |  Usuario. |
| Descripción | El usuario accede a su historial de préstamos y devoluciones.|
| Flujo básico | 1-> El usuario inicia sesión en el sistema. 2-> El usuario accede a su historial de préstamos y devoluciones.|
| Pre-condiciones | El usuario está autenticado en el sistema.|  
| Post-condiciones  | El usuario ha visualizado su historial de préstamos y devoluciones.|  
|  Requerimientos | El usuario debe tener préstamos o devoluciones registrados.|
|  Notas | Puede incluir detalles adicionales sobre la información que se mostrará.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |

#### 6. Gestionar Inventario:

|  Caso de Uso	CU | Gestionar Inventario  |
|---|---|
| Fuentes  | gestión de biblioteca |
| Actor  |  Bibliotecario. |
| Descripción |El bibliotecario puede agregar, modificar o eliminar libros del inventario.|
| Flujo básico |1-> El bibliotecario inicia sesión en el sistema. 2-> El bibliotecario accede a la sección de gestión de inventario. 3-> El bibliotecario realiza las acciones necesarias (agregar, modificar o eliminar libros).|
| Pre-condiciones | El bibliotecario está autenticado en el sistema.|  
| Post-condiciones  | El inventario se actualiza según las acciones realizadas por el bibliotecario.|  
|  Requerimientos | Ninguno en particular |
|  Notas | Puede incluir detalles adicionales sobre las acciones permitidas.|
| Autor  | Eduardo Rabadán Melián |
|Fecha | 23/01/2024 |
