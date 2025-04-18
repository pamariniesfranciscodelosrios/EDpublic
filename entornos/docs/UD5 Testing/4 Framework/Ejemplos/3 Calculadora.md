## 4.1 Ejercicio Teoría Ahora tu

Creamos proyecto llamado **"Calculadora"** en una ruta que tengamos para Entornos de Desarrollo de GitHub.

![1743262210195](image/EjercicioAhoratu/1743262210195.png)

- Subimos a repositorio **Github** Entornos Desarrollo/UD5/Calculadora
- Subimos el **enlace repositorio** a tarea Moodle

![1743262076644](image/EjercicioAhoratu/1743262076644.png)

### Codigo:

```java
package dam.ed;

public class Calculadora {

    double suma(double a, double b) {
        return a + b;
    }

    double resta(double minuendo, double sustraendo) {
        return minuendo - sustraendo;
    }

    double multiplica(double a, double b) {
        return Math.abs(a * b);
    }

    double divide(double dividendo, double divisor) throws Exception {
        if (divisor == 0) {
            throw new Exception("El divisor es 0");
        }
        return dividendo / divisor;
    }

    double potencia(double base, double exponente) {
        return Math.pow(base, exponente);
    }
}
```

### Seleccionar Generar Test en el IDE (Alt + ENTER)

![1743262745421](image/EjercicioAhoratu/1743262745421.png)

### Crear test

![1743262802686](image/EjercicioAhoratu/1743262802686.png)

### Ejecuta test

![1743263248298](image/EjercicioAhoratu/1743263248298.png)

### Errores en la ejecución

![1743264231678](image/EjercicioAhoratu/1743264231678.png)

### Tras la corrección

![1743264557307](image/EjercicioAhoratu/1743264557307.png)

## Referencias:

- teoría UD5
- [Documentación JetBrains](https://www.jetbrains.com/help/idea/performing-tests.html#run-tests)
- ![1743263158066](image/EjercicioAhoratu/1743263158066.png)
