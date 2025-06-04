# 🏀 Estructura Condicionale IF-ELIF-ELSE en Python

Primer ejercicio de la cátedra.

## 📋 Contenido

### Conceptos Cubiertos
- `if` simple
- `if-else` (condicional doble)
- `if-elif-else` (condicional múltiple)
- Operadores de comparación (`<`, `<=`, `>=`, `>`, `==`, `!=`)
- Rangos de valores
- Anidamiento de condicionales

## 🎯 Ejercicio Incluido:

### IF-ELSE-ELIF 1.py - Clasificador de Posiciones de Baloncesto
Determina la posición de un jugador según su altura:

```python
# Clasificación por altura
Menos de 160 cm     → Base
160 - 179 cm        → Escolta  
180 - 199 cm        → Alero
200 cm o más        → Pivot
```

**Características del programa:**
- Entrada: Altura en centímetros (float)
- Salida: Posición en la cancha
- Uso de rangos con operadores `<=` y `>=`
- Estructura `if-elif-else` en cascada

## 🔧 Conceptos Técnicos Aplicados

### Operadores de Comparación
```python
altura < 160                    # Menor que
160 <= altura <= 179           # Rango inclusivo
altura >= 200                  # Mayor o igual que
```

### Estructura Condicional Múltiple
```python
if condicion1:
    # Acción 1
elif condicion2:
    # Acción 2  
elif condicion3:
    # Acción 3
else:
    # Acción por defecto
```

## 🎲 Casos de Prueba

| Altura (cm) | Posición Esperada |
|-------------|-------------------|
| 150         | Base             |
| 165         | Escolta          |
| 185         | Alero            |
| 210         | Pivot            |

## 🚀 Cómo Ejecutar

1. Clona el repositorio
2. Ejecuta IF-ELSE-ELIF 1 `.py`:
   ```bash
   python "IF-ELSE-ELIF 1.py"
   ```
3. Ingresa la altura cuando se solicite
4. Observa la clasificación resultado

## 📚 Fundamentos de Programación

Este proyecto sigue principios de programación algorítmica:
- **Entrada-Proceso-Salida**: Estructura clara del algoritmo
- **Validación implícita**: Manejo de rangos numéricos
- **Legibilidad**: Código claro y bien estructurado
- **Casos exhaustivos**: Cobertura completa de rangos

## 🎓 Objetivos de Aprendizaje

Al completar este ejercicio, aprendí a:
- ✅ Implementar decisiones lógicas en código
- ✅ Usar operadores de comparación efectivamente  
- ✅ Estructurar condicionales múltiples
- ✅ Manejar rangos numéricos
- ✅ Crear programas interactivos con entrada de usuario

## 🔗 Conceptos Relacionados

- Variables y tipos de datos (float, string)
- Entrada y salida por consola (`input()`, `print()`)
- Casting de tipos (`float()`)
- Operadores lógicos y relacionales

---

*Ejercicio desarrollado por Lautaro Fernandez como parte del aprendizaje de Programación I - Estructuras de Control.*
