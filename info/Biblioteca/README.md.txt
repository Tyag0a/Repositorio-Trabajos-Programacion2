2. Sistema de Gestión de Biblioteca
Contexto: En un sistema de gestión de biblioteca, se necesita gestionar libros, miembros, préstamos y multas, así como el personal que atiende la biblioteca.
Clases:
Libro: Atributos incluye título, autor, ISBN, y estado (disponible o prestado).
Miembro: Atributos incluyen nombre, ID de miembro, y una lista de préstamos activos.
Préstamo: Relaciona un libro con un miembro, incluyendo los atributos fecha de préstamo y fecha de devolución.
Empleado: Clase base para el personal con atributos como nombre y ID de empleado.
Bibliotecario: Hereda de Empleado, añade métodos específicos como gestionarPréstamos().
Relaciones:
Un Miembro puede tener varios Préstamos.
Un Préstamo está asociado a un Libro y a un Miembro.
Un Bibliotecario puede gestionar múltiples Libros y Préstamos.
Herencia:
Bibliotecario hereda de Empleado.
Polimorfismo:
Podríamos tener una interfaz GestiónInventario que Bibliotecario implemente para gestionar diferentes tipos de ítems de la biblioteca (libros, revistas, DVDs), utilizando el método gestionarItem() de manera polimórfica.