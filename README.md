# 💱 Conversor de Divisas y Temperaturas - Challenge Java (Oracle ONE / Alura Latam)

<p>
  <img align="left" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" alt="Java" />
  <img align="left" src="https://img.shields.io/badge/Oracle_ONE-F80000?style=for-the-badge&logo=oracle&logoColor=white" alt="Oracle ONE" />
  <img align="left" src="https://img.shields.io/badge/Alura_Latam-007ACC?style=for-the-badge&logo=vlc&logoColor=white" alt="Alura Latam" />
  <img align="left" src="https://img.shields.io/badge/Estado-Completado-success?style=for-the-badge" alt="Estado: Completado" />
</p>
<br clear="all">

¡Bienvenido al **Conversor de Divisas y Temperaturas**! Este proyecto fue desarrollado como parte del **Challenge de Java** del programa **Oracle Next Education (ONE)** en colaboración con **Alura Latam**. 

Se trata de una aplicación de escritorio desarrollada en **Java** con interfaz gráfica interactiva (**Java Swing** via `JOptionPane`), que permite realizar conversiones precisas entre múltiples divisas internacionales y escalas de temperatura, garantizando una experiencia visual amigable y un control de errores riguroso.

---

## 🚀 Características Principales

### 💵 1. Conversor de Divisas
Permite convertir de forma bidireccional entre la moneda local (Pesos) y las principales divisas del mundo:
- **Pesos** ↔️ **Dólares (USD)**
- **Pesos** ↔️ **Euros (EUR)**
- **Pesos** ↔️ **Libras Esterlinas (GBP)**
- **Pesos** ↔️ **Yen Japonés (JPY)**
- **Pesos** ↔️ **Won Surcoreano (KRW)**

*Formateo preciso a dos decimales (`DecimalFormat`) y cálculo bidireccional automático.*

### 🌡️ 2. Conversor de Temperaturas
Soporta las 3 escalas térmicas más utilizadas a nivel global con conversión en ambos sentidos:
- **Celsius (°C)** ↔️ **Fahrenheit (°F)**
- **Celsius (°C)** ↔️ **Kelvin (K)**
- **Fahrenheit (°F)** ↔️ **Kelvin (K)**

### 🛡️ 3. Validación y Control de Errores
- **Excepción Personalizada (`NegativeNumberException`)**: Impide el ingreso de montos o valores menores o iguales a cero en el conversor de divisas.
- **Validación de Entradas Vacías**: Detecta cuando el usuario no ingresa ningún valor o presiona aceptar sin completar el campo.
- **Manejo de Errores de Formato (`NumberFormatException`)**: Captura caracteres alfabéticos o símbolos no numéricos informando adecuadamente al usuario.

### 🎨 4. Interfaz Gráfica Personalizada (GUI)
- Construido con cuadros de diálogo modales e intuitivos mediante `javax.swing.JOptionPane`.
- **Iconografía adaptada**: Incorpora imágenes e íconos personalizados (`doubt`, `foreignExchange`, `conversion`, `amount`, `error`, `thanks`) para enriquecer la experiencia visual.
- **Ciclo Interactivo**: Permite realizar múltiples operaciones consecutivas mediante diálogos de confirmación (`YES_NO_OPTION`).

---

## 🛠️ Tecnologías Utilizadas

### ☕ Lenguaje
<p>
  <img align="left" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
</p>
<br clear="all">

### 🖥️ Interfaz Gráfica
<p>
  <img align="left" src="https://img.shields.io/badge/Java_Swing-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java Swing" />
  <img align="left" src="https://img.shields.io/badge/JOptionPane-007396?style=for-the-badge&logo=openjdk&logoColor=white" alt="JOptionPane" />
</p>
<br clear="all">

### 📐 Paradigma & Prácticas
<p>
  <img align="left" src="https://img.shields.io/badge/POO-0052CC?style=for-the-badge&logo=java&logoColor=white" alt="Programación Orientada a Objetos" />
  <img align="left" src="https://img.shields.io/badge/Manejo_de_Excepciones-DC143C?style=for-the-badge&logo=java&logoColor=white" alt="Manejo de Excepciones" />
  <img align="left" src="https://img.shields.io/badge/DecimalFormat-5C5C5C?style=for-the-badge&logo=java&logoColor=white" alt="DecimalFormat" />
</p>
<br clear="all">

### 🛠️ IDEs Recomendadas
<p>
  <img align="left" src="https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white" alt="VS Code" />
  <img align="left" src="https://img.shields.io/badge/IntelliJ_IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=white" alt="IntelliJ IDEA" />
  <img align="left" src="https://img.shields.io/badge/Eclipse-2C2255?style=for-the-badge&logo=eclipseide&logoColor=white" alt="Eclipse" />
</p>
<br clear="all">

---

## 📁 Estructura del Proyecto

```text
Conversor de divisas/
│
├── bin/                          # Archivos compilados (.class)
├── src/                          # Código fuente del proyecto
│   ├── App.java                  # Clase principal con menú y lógica de conversión
│   ├── NegativeNumberException.java # Excepción custom para validación de montos
│   └── img/                      # Recursos de imagen/íconos para la GUI
│       ├── amount.png            # Ícono para ingreso de montos
│       ├── conversion.png        # Ícono para resultado de conversión
│       ├── doubt.png             # Ícono para selección inicial
│       ├── error.png             # Ícono para mensajes de error
│       ├── foreignExchange.png   # Ícono para selección de divisas
│       └── thanks.png            # Ícono de despedida/agradecimiento
│
└── README.md                     # Documentación del proyecto
```

---

## 💻 Requisitos e Instalación

### Prerrequisitos
- Tener instalado **Java Development Kit (JDK 8)** o superior.
- (Opcional) Un IDE de desarrollo Java (VS Code, IntelliJ IDEA, Eclipse, etc.).

### Ejecución desde la Terminal

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/GustavoBaranda/Challenge-Oracle-ONE.git
   cd "Conversor de divisas"
   ```

2. **Compilar el proyecto:**
   ```bash
   javac -d bin src/*.java
   ```

3. **Ejecutar la aplicación:**
   ```bash
   java -cp bin App
   ```

---

## 📐 Lógica de Negocio y Fórmulas

### Conversor de Temperaturas
Las fórmulas empleadas para las conversiones entre escalas térmicas son:
- **Celsius a Fahrenheit**: $T_{°F} = \left(T_{°C} \times \frac{9}{5}\right) + 32$
- **Fahrenheit a Celsius**: $T_{°C} = (T_{°F} - 32) \times \frac{5}{9}$
- **Celsius a Kelvin**: $T_{K} = T_{°C} + 273.15$
- **Kelvin a Celsius**: $T_{°C} = T_{K} - 273.15$
- **Fahrenheit a Kelvin**: $T_{K} = (T_{°F} - 32) \times \frac{5}{9} + 273.15$
- **Kelvin a Fahrenheit**: $T_{°F} = (T_{K} - 273.15) \times \frac{9}{5} + 32$

---

## 🌟 Reconocimientos y Créditos

Este proyecto fue realizado como entrega del desafío de Java dentro de la especialización de **Backend** de **Oracle Next Education (ONE)** en conjunto con **Alura Latam**.

- **Desarrollador**: [Gustavo Baranda](https://github.com/GustavoBaranda)
- **Programa**: Oracle Next Education (ONE) / Alura Latam
