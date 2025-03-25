# POO I (Programación Orientada a Objetos I)

Este repositorio contiene ejercicios fundamentales de Programación Orientada a Objetos en Java, orientados a principiantes. Se trabajan conceptos como encapsulación, herencia, polimorfismo, interfaces y composición. Sirve como base para iniciarse en la programación con Java orientada a objetos.

---

## 🔧 Estructura del proyecto

El código está organizado por paquetes según los temas trabajados:

- **modelo:** Clases que representan entidades del dominio  
  (`Persona.java`, `Empleado.java`, `Cliente.java`, `Producto.java`, `Factura.java`)

- **interfaces:** Define contratos para comportamientos  
  (`Trabajador.java`, `Vendedor.java`)

- **herenciaPolimorfismo:** Ejemplos de herencia y polimorfismo  
  (`Animal.java`, `Perro.java`, `Gato.java`)

---

## 🚀 Cómo usar este proyecto

1. Clona el repositorio:
   ```bash
   git clone https://github.com/ManoloMiranda-11/POO_I.git
   ```
2. Abre el proyecto en Eclipse, IntelliJ u otro IDE que soporte Java.
3. Explora las clases dentro de la carpeta `src/` para ver la estructura y ejemplos.
4. (Opcional) Crea una clase `Test` para probar el funcionamiento de las clases.

---

### 📌 Requisitos

- JDK 11 o superior.
- Eclipse, IntelliJ u otro IDE que soporte Java.
- Git instalado (opcional si descargas el proyecto como ZIP).

---

## 📘 Recursos útiles

- [Documentación oficial de Java](https://docs.oracle.com/en/java/)
- [Tutorial de POO en Java (YouTube)](https://www.youtube.com/playlist?list=PLWtYZ2ejMVJlUu5lq2d3xE6Cs4t73zvPp)

---

## ✍️ Ejemplo de código

```java
// Ejemplo de uso de clases con herencia y polimorfismo

public abstract class Persona {
    protected String nombre;

    public Persona(String nombre) {
        this.nombre = nombre;
    }

    public abstract void presentarse();
}

public class Empleado extends Persona {
    private String puesto;

    public Empleado(String nombre, String puesto) {
        super(nombre);
        this.puesto = puesto;
    }

    @Override
    public void presentarse() {
        System.out.println("Hola, soy " + nombre + " y trabajo como " + puesto + ".");
    }
}

public class Main {
    public static void main(String[] args) {
        Persona p = new Empleado("Laura", "desarrolladora");
        p.presentarse();
    }
}
```

---

## 📂 Estructura de carpetas

```
POO_I/
│
├── src/
│   ├── modelo/
│   │   ├── Persona.java
│   │   ├── Empleado.java
│   │   ├── Cliente.java
│   │   ├── Producto.java
│   │   └── Factura.java
│   ├── interfaces/
│   │   ├── Trabajador.java
│   │   └── Vendedor.java
│   └── herenciaPolimorfismo/
│       ├── Animal.java
│       ├── Perro.java
│       └── Gato.java
│
└── README.md
```
