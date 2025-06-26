# MODULO2_Ejercicios-pr-cticos-de-Clases-y-Objetos3
Ejercicios prácticos de Clases y Objetos (CodeRunner)


En el siguiente ejercicio, se te pide que implementes una clase en Java para representar un estudiante. La clase debe tener los siguientes atributos y métodos:

Atributos:

nombre (String): el nombre del estudiante.
edad (int): la edad del estudiante.
nota (double): la nota del estudiante.
Métodos:

getNombre(): devuelve el nombre del estudiante.
getEdad(): devuelve la edad del estudiante.
getNota(): devuelve la nota del estudiante.
setNombre(String nombre): establece el nombre del estudiante.
setEdad(int edad): establece la edad del estudiante.
setNota(double nota): establece la nota del estudiante.
toString(): devuelve una cadena que representa el estudiante en el formato "Nombre: [nombre], Edad: [edad], Nota: [nota]".
Implementa la clase Estudiante de acuerdo con los requisitos mencionados.


Por ejemplo:

Prueba	Resultado
Estudiante estudiante1 = new Estudiante();
estudiante1.setNombre("Juan");
estudiante1.setEdad(20);
estudiante1.setNota(85.5);
System.out.println(estudiante1.toString());
Nombre: Juan, Edad: 20, Nota: 85.5

-------------------------------------------------------------

// public class Estudiante {
    // Atributos
    private String nombre;
    private int edad;
    private double nota;

    // Constructor por defecto
    public Estudiante() {
        this.nombre = "";
        this.edad = 0;
        this.nota = 0.0;
    }

    // Métodos getters
    public String getNombre() {
        return nombre;
    }

    public int getEdad() {
        return edad;
    }

    public double getNota() {
        return nota;
    }

    // Métodos setters
    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public void setEdad(int edad) {
        this.edad = edad;
    }

    public void setNota(double nota) {
        this.nota = nota;
    }

    // Método toString
    @Override
    public String toString() {
        return "Nombre: " + nombre + ", Edad: " + edad + ", Nota: " + nota;
    }
}
