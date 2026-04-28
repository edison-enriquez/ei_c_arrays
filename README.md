# ei_c_arrays

En C, el **bucle `for`** se usa para repetir un bloque de código un número determinado de veces. Es especialmente útil cuando sabes cuántas iteraciones necesitas.

### 📌 Estructura básica

```c
for (inicialización; condición; incremento) {
    // código que se repite
}
```

### 🔍 ¿Qué hace cada parte?

* **Inicialización**: se ejecuta una sola vez al inicio (por ejemplo, definir un contador).
* **Condición**: se evalúa antes de cada iteración; si es verdadera, el bucle continúa.
* **Incremento (o actualización)**: se ejecuta después de cada vuelta del bucle.

---

### ✅ Ejemplo simple

```c
#include <stdio.h>

int main() {
    for (int i = 0; i < 5; i++) {
        printf("Valor de i: %d\n", i);
    }
    return 0;
}
```

### 🧠 ¿Qué pasa aquí?

1. `int i = 0;` → empieza en 0
2. `i < 5` → se repite mientras i sea menor que 5
3. `i++` → aumenta i en 1 cada vez

🔁 Resultado:

```
Valor de i: 0
Valor de i: 1
Valor de i: 2
Valor de i: 3
Valor de i: 4
```

---

### ⚡ Variaciones útiles

✔ Contar hacia atrás:

```c
for (int i = 5; i > 0; i--) {
    printf("%d\n", i);
}
```

✔ Incrementos diferentes:

```c
for (int i = 0; i <= 10; i += 2) {
    printf("%d\n", i); // imprime pares
}
```

✔ Sin alguna parte (aunque no es común):

```c
int i = 0;
for (; i < 5; ) {
    printf("%d\n", i);
    i++;
}
```

---

### 🚨 Cuidado

Si la condición nunca se vuelve falsa, tendrás un **bucle infinito**:

```c
for (int i = 0; i >= 0; i++) {
    // nunca termina
}
```

---

Si quieres, puedo mostrarte ejercicios típicos con `for` (como tablas de multiplicar o recorrer arreglos) para que lo practiques.
