##PATRONES DE DISEÑO
##TALLER EN CLASE
##PROBLEMATICA
Pepito es un Ingeniero de Software Junior en Codificando Con Patrones Cía. Ltda. Se le ha encargado la tarea de completar los requerimientos funcionales del aplicativo de automóviles al que la empresa da soporte. 

Los requisitos son los siguientes: 

- Implementar los métodos de agregar vehículos (add Mustang y add Explorer) en el Home Page. El programador anterior implementó un patrón repositorio que contiene los métodos CRUD para el repositorio de automóviles; sin embargo, el equipo de QA ha reportado que no funciona como se espera. 
 

- El equipo de base de datos ha comentado que el esquema de la base de datos no está listo. Por lo que se necesita buscar una forma de probar la funcionalidad sin tener que guardar en la base de datos, de tal forma que después se implemente la funcionalidad de base de datos cuando esté lista. 

- El equipo de negocio ha solicitado agregar el año actual, y 20 propiedades más por defecto que se solicitarán en el siguiente sprint. Estas propiedades afectan a vehículo. Implementa un patrón de diseño para agregar propiedades por defecto, y como lo diseñarías para minimizar los cambios para el siguiente sprint. 

- Se planea agregar un nuevo modelo. El Arquitecto de Software prevee que la unidad de negocio, planeará la introducción de más modelos por lo cual sugiere la implementación de un Factory Method. 

  - Color: Red 

  - Marca: Ford 

  - Modelo: Escape
 
  Patrón Singleton
El patrón Singleton se utiliza para garantizar que una clase tenga una única instancia y proporciona un punto global de acceso a esa instancia. Esto es útil cuando exactamente una instancia de una clase es necesaria para coordinar acciones en todo el sistema.
Cómo funciona:
Constructor Privado: La clase Singleton tiene un constructor privado para evitar que se creen instancias directamente desde fuera de la clase.
Instancia Única: La clase tiene una variable privada que almacena la única instancia de la clase.
Método Estático de Acceso: Proporciona un método estático que actúa como punto de acceso global a la instancia única de la clase. Si la instancia aún no existe, se crea; de lo contrario, se devuelve la instancia existente.
![image](https://github.com/whosnnck/DesignPatternsUDLA/assets/131733484/265b0351-eff4-4612-be47-f245c9b30f0d)
 

Estructura del Patrón Singleton
Patrón Builder
El patrón Builder es un patrón creacional que se utiliza para construir un objeto complejo paso a paso. Permite construir diferentes representaciones de un objeto utilizando el mismo proceso de construcción. Este patrón se centra en la construcción de un producto complejo paso a paso. Es útil cuando la construcción de un objeto es complicada, y se desea tener control sobre cada paso del proceso.

Cómo funciona:
Director: Clase que coordina el proceso de construcción utilizando un objeto Builder. El Director no sabe cómo se construye el producto, solo sabe cómo utilizar el Builder para construirlo.
Builder: Define una interfaz para construir las partes del producto. Tiene métodos para construir cada parte del producto, como construir la base, las paredes y el techo.
ConcreteBuilder: Implementa la interfaz del Builder y construye las partes específicas del producto. Conoce los detalles de implementación y construcción del producto.
Producto: El objeto complejo que se está construyendo. Puede tener varias partes y características.
![image](https://github.com/whosnnck/DesignPatternsUDLA/assets/131733484/c6351451-9399-4441-be0d-05398dba387e)


Estructura del Patrón Builder
Patrón Factory Method
El patrón de diseño Factory Method se utiliza cuando una clase no puede anticipar la clase de objetos que debe crear. En lugar de crear directamente un objeto, delega la responsabilidad a sus subclases. Este patrón define una interfaz para crear un objeto, pero deja que las subclases alteren el tipo de objetos que se crearán. Es un patrón creacional que proporciona una interfaz para crear instancias de una clase, pero permite a las subclases alterar el tipo de instancias que se crearán.
Cómo funciona:
Interfaz o Clase Abstracta: Define una interfaz o clase abstracta que declara el método abstracto (Factory Method) para crear un producto. Este método puede contener una implementación básica compartida por todas las subclases.
Subclases: Implementan el Factory Method para crear instancias concretas del producto. Cada subclase puede proporcionar una implementación diferente del Factory Method, creando así diferentes variantes del producto.
Cliente: Utiliza el Factory Method para crear instancias del producto sin conocer la clase concreta del producto. Esto permite que el cliente sea independiente de las clases concretas y hace que el código sea más flexible y fácil de extender.
![image](https://github.com/whosnnck/DesignPatternsUDLA/assets/131733484/6d9f3e67-cdba-4606-b164-fe53ce449638)

Estructura del Patrón Facthory Method

Referencia
- https://refactoring.guru/design-patterns

