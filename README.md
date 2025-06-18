# 📚 Guía 1: Estructuras Condicionales en Python

## 🎯 Descripción del Proyecto

Este repositorio contiene los ejercicios desarrollados para la **Guía 1 de Programación I** en la Universidad Tecnológica Nacional (UTN). Los ejercicios se enfocan en el dominio de estructuras condicionales, validación de datos y lógica de control de flujo en Python.

## 🚀 Tecnologías Utilizadas

- **Python 3.10**
- Estructuras condicionales (`if`, `elif`, `else`)
- Sentencias `match-case` (Python 3.10+)
- Operadores lógicos y de comparación
- Funciones de entrada/salida (`input()`, `print()`)
- Formateo de strings y manejo de tipos de datos

## 📁 Estructura del Proyecto

```
├── Gotita.py              # Sistema de facturación de servicios públicos
├── IF-ELSE-ELIF 1.py      # Clasificador de posiciones en baloncesto
├── IF-ELSE-ELIF 2.py      # Evaluador de calificaciones académicas
├── Match.py               # Sistema de destinos turísticos por estación
└── README.md              # Documentación del proyecto
```

## 🔍 Ejercicios Desarrollados

### 1. **Sistema de Facturación de Servicios Públicos** (`Gotita.py`)
**Complejidad:** ⭐⭐⭐⭐

Sistema completo de facturación que calcula el costo de servicios públicos considerando:
- **Tipos de cliente:** Residencial, Comercial, Industrial
- **Tarifas diferenciadas:** Cargo fijo + consumo variable
- **Bonificaciones y recargos** según rangos de consumo
- **Descuentos especiales** para clientes residenciales
- **Cálculo de IVA** y generación de factura detallada

**Conceptos aplicados:**
- Estructuras `match-case` anidadas
- Validación de entrada de datos
- Cálculos financieros complejos
- Formateo numérico profesional

| Tipo Cliente | Consumo (m³) | Bonificación/Recargo | Ejemplo Cálculo |
|--------------|--------------|---------------------|-----------------|
| Residencial  | 25           | 10% bonificación    | $5,000 → $4,500 |
| Comercial    | 400          | 12% bonificación    | $80,000 → $70,400 |
| Industrial   | 100          | 10% recargo         | $20,000 → $22,000 |
| Residencial  | 15 (factura <$35k) | 5% desc. especial | + descuento adicional |

### 2. **Clasificador de Posiciones en Baloncesto** (`IF-ELSE-ELIF 1.py`)
**Complejidad:** ⭐⭐

Determina la posición de un jugador basándose en su altura:
- Base: < 160 cm
- Escolta: 160-179 cm  
- Alero: 180-199 cm
- Pivot: ≥ 200 cm

**Conceptos aplicados:**
- Cadenas de `if-elif-else`
- Operadores de comparación
- Rangos numéricos

| Altura (cm) | Posición Esperada |
|-------------|-------------------|
| 150         | Base              |
| 165         | Escolta           |
| 185         | Alero             |
| 210         | Pivot             |

### 3. **Evaluador de Calificaciones Académicas** (`IF-ELSE-ELIF 2.py`)
**Complejidad:** ⭐⭐

Sistema de evaluación académica que clasifica notas del 1-10:
- Promoción directa: 6-10
- Aprobado: 4-5
- Desaprobado: 1-3

**Conceptos aplicados:**
- Validación de rangos
- Lógica condicional simple
- Manejo de casos edge

| Nota | Resultado |
|------|-----------|
| 9    | Promoción directa |
| 4    | Aprobado |
| 2    | Desaprobado |
| 11   | Monto inválido |

### 4. **Sistema de Destinos Turísticos** (`Match.py`)
**Complejidad:** ⭐⭐⭐

Determina disponibilidad de viajes según estación del año:
- **Invierno:** Solo Bariloche
- **Verano:** Mar del Plata y Cataratas
- **Otoño:** Todos los destinos
- **Primavera:** Todos excepto Bariloche

**Conceptos aplicados:**
- Sentencias `match-case`
- Lógica booleana compleja
- Procesamiento de strings
- Manejo de múltiples condiciones

| Estación | Destino | ¿Se viaja? |
|----------|---------|------------|
| Invierno | Bariloche | ✅ Sí |
| Invierno | Cataratas | ❌ No |
| Verano | Mar del Plata | ✅ Sí |
| Otoño | Cualquiera | ✅ Sí |
| Primavera | Bariloche | ❌ No |

## 💡 Habilidades Desarrolladas

### Técnicas de Programación
- ✅ **Control de flujo ** con estructuras condicionales
- ✅ **Validación de datos simple** de tipo entrada
- ✅ **Diseño de algoritmos** para resolver problemas del mundo real
- ✅ **Optimización de código** usando `match-case` vs `if-elif`

### Buenas Prácticas
- ✅ **Nomenclatura clara** y descriptiva de variables
- ✅ **Comentarios explicativos** para lógica compleja
- ✅ **Formateo consistente** del código
- ✅ **Manejo de casos especiales** y validaciones

### Resolución de Problemas
- ✅ **Análisis de requerimientos** complejos (sistema de facturación)
- ✅ **Modelado de lógica de negocio** real
- ✅ **Implementación de cálculos** precisos
- ✅ **Diseño de interfaces de usuario** por consola

## 🔧 Cómo Ejecutar

1. **Clonar el repositorio:**
```bash
git clone https://github.com/ferlautaro2001/1--Condicionales.git
cd programacion1-condicionales
```

2. **Ejecutar cualquier ejercicio:**
```bash
python Gotita.py
python IF-ELSE-ELIF 1.py
python IF-ELSE-ELIF 2.py
python Match.py
```

## 📊 Casos de Prueba Sugeridos

### Para `Gotita.py`:
- Cliente residencial, 25 m³ (debe aplicar bonificación)
- Cliente comercial, 400 m³ (debe aplicar bonificación del 12%)
- Cliente industrial, 100 m³ (debe aplicar recargo del 10%)

| Escenario | Entrada | Resultado Esperado |
|-----------|---------|-------------------|
| Residencial bajo consumo | 25 m³ | Bonificación 10% |
| Comercial alto consumo | 400 m³ | Bonificación 12% |
| Industrial medio consumo | 100 m³ | Recargo 10% |
| Residencial con desc. especial | 15 m³ | Bonificación + 5% adicional |

### Para otros ejercicios:
- Valores límite de cada rango
- Casos fuera de rango para validar robustez

| Ejercicio | Caso Límite | Entrada | Salida Esperada |
|-----------|-------------|---------|-----------------|
| Baloncesto | Límite Base-Escolta | 160 cm | Escolta |
| Calificaciones | Límite Aprobado-Promoción | 6 | Promoción directa |
| Turismo | Destino inexistente | "París" | Manejo de error |

## 🎓 Aprendizajes Clave

En esta guía aprendí a:
- **Traducir problemas complejos** del mundo real a código funcional.
- **Implementar lógica** con múltiples variables y condiciones.
- **Crear sistemas básicos** con validación de entradas simples.
- **Comentar y estructurar código** de manera prolija.

## 👨‍💻 Autor

**Lautaro Fernandez**  
Estudiante de Programación 1 - Universidad Tecnológica Nacional  

---

*Desarrollado como parte de la cátedra de Programación 1 en UTN - Abril 2025*
