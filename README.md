# Informe Final del Proyecto: Pruebas y Documentación para la Función "Compartir un Automóvil"

## **Descripción del Proyecto**
Este proyecto se enfocó en analizar y documentar los requisitos de la función **"Compartir un automóvil"** de la aplicación **Urban Routes**. Las actividades incluyeron la creación de documentación técnica y pruebas para las funcionalidades relacionadas con:

- **Adición de licencias de conducir.**
- **Cálculo del precio y duración del viaje.**

---

## **Objetivos**
1. Diseñar un mapa mental para visualizar los requisitos y validaciones de la función "Agregar licencia de conducir".
2. Definir **clases de equivalencia** y **valores límite** para los campos "Nombre" y "Apellido" del formulario de licencia.
3. Elaborar un **diagrama de flujo** que describa la lógica del cálculo de precio y duración en la funcionalidad de "Compartir un automóvil".

---

## **Desarrollo del Proyecto**

### **1. Mapa Mental: Función "Agregar Licencia de Conducir"**
El mapa mental incluye:
- **Sección de Entrada de Datos:**
  - Campos: `Nombre`, `Apellido`, `Número de Licencia`, `Fecha de Vencimiento`, `País de Expedición`.
  - Validaciones:
    - Obligatorio para todos los campos.
    - Formato válido para el número de licencia.
    - Fecha de vencimiento no puede ser anterior a la fecha actual.
- **Validaciones en Tiempo Real:**
  - Mensajes de error claros y específicos.
  - Indicadores visuales para retroalimentación inmediata.
- **Mensajes de Confirmación:**
  - Éxito al agregar una licencia.
  - Notificación de errores por datos incompletos o inválidos.

### **2. Clases de Equivalencia y Valores Límite**
#### **Campo "Nombre":**
- **Clases de Equivalencia:**
  - **Válido:** Solo letras, longitud entre 1 y 50 caracteres.
  - **Inválido:** Incluye números, caracteres especiales o excede 50 caracteres.
- **Valores Límite:**
  - Límite inferior: `"A"` (1 carácter).
  - Límite superior: `"NombreDePruebaCon50CaracteresExactos"`.

#### **Campo "Apellido":**
- **Clases de Equivalencia:**
  - **Válido:** Solo letras, longitud entre 1 y 50 caracteres.
  - **Inválido:** Incluye números, caracteres especiales o excede 50 caracteres.
- **Valores Límite:**
  - Límite inferior: `"B"` (1 carácter).
  - Límite superior: `"ApellidoDePruebaCon50CaracteresExactos"`.

### **3. Diagrama de Flujo: Cálculo del Precio y Duración del Viaje**
El diagrama de flujo detalla los siguientes pasos:
1. **Entrada de Datos:**
   - Dirección de inicio y destino.
   - Número de pasajeros.
2. **Cálculo de Distancia:**
   - Obtener la distancia entre los puntos.
   - Validar que la distancia sea mayor a 0.
3. **Selección de Vehículo:**
   - Tipo de transporte compartido (e.g., automóvil, bicicleta).
4. **Cálculo del Precio:**
   - Fórmula: `(Distancia x Tarifa Base) + (Costo por Pasajero x Número de Pasajeros)`.
   - Aplicar descuentos según las condiciones.
5. **Cálculo de Duración:**
   - Fórmula: `Distancia / Velocidad Promedio`.
   - Agregar tiempo extra para más de un pasajero.
6. **Validaciones Finales:**
   - Revisar que no existan valores negativos o incoherentes.
7. **Salida:**
   - Mostrar precio y duración estimados al usuario.

---

## **Resultados**
1. **Mapa Mental:** Documenta de manera gráfica los flujos y validaciones de la función "Agregar licencia de conducir".
2. **Clases de Equivalencia y Valores Límite:** Proporcionan un marco sólido para diseñar casos de prueba exhaustivos.
3. **Diagrama de Flujo:** Facilita la comprensión de la lógica de cálculo y posibles errores en el proceso.

---
**Enlace a los reportes finales:** [[Ver Informe Final](https://drive.google.com/drive/folders/11OWBd9FbJMgfMAItTpAU-hTISpfQSERe?usp=sharing)](#)
---

## **Recomendaciones**
1. Implementar validaciones adicionales para evitar errores en campos sensibles como "Nombre" y "Apellido".
2. Diseñar y ejecutar casos de prueba utilizando las clases de equivalencia y valores límite definidos.
3. Automatizar las pruebas del cálculo de precio y duración utilizando herramientas como Selenium o Cypress.

---

**Equipo QA de Urban Routes**  


---
