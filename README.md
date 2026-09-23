# ⚛️ CuànticLAB — Entrenador de Números Cuánticos y Orbitales Atómicos

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deploy-success?style=flat&logo=github)](https://pages.github.com/)
[![Nivel Educativo](https://img.shields.io/badge/Qu%C3%ADmica-2%C2%BA%20Bachillerato-indigo)](#)
[![Orientación](https://img.shields.io/badge/Preparaci%C3%B3n-PAU%20%2F%20Selectividad-blue)](#)
[![Idiomas](https://img.shields.io/badge/Idiomas-Castellano%20%7C%20Catal%C3%A0-orange)](#)
[![Licencia](https://img.shields.io/badge/Licencia-CC%20BY--NC--SA%204.0-lightgrey)](#)

**CuànticLAB** es una aplicación web interactiva diseñada como recurso docente para la materia de **Química de 2.º de Bachillerato**. Su objetivo es facilitar el entrenamiento activo, la deducción de números cuánticos, la visualización geométrica tridimensional de orbitales atómicos y la correcta justificación formal en cuestiones de la **Prueba de Acceso a la Universidad (PAU / Selectividad)**.

---

## 🎯 Finalidad y Características Pedagógicas

1. **Entrenador Cuántico Bidireccional (escritura directa por teclado):**
   - **$(n, l, m_l, m_s) \rightarrow \text{Orbital}$:** Deducción del subnivel orbital a partir de una cuaterna dada (ej. $n=4, l=2 \rightarrow 4d$).
   - **$\text{Orbital} \rightarrow (n, l, m_l)$:** Identificación del nivel principal $n$ y el número azimutal $l$ a partir de la notación espectroscópica.
   - **Modo Mixto:** Alternancia aleatoria de retos para fomentar la flexibilidad cognitiva del alumnado.
   - Entrada mediante teclado con soporte completo para la tecla `Enter`, evitando pistas visuales prematuras en los campos de texto.

2. **Módulo de Examen PAU: ¿Válido o Prohibido?:**
   - Planteamiento de cuaternas aleatorias para evaluar su viabilidad física.
   - Justificación automática escalonada según los criterios de corrección oficiales de las comisiones de Química de selectividad ($n \ge 1$, $0 \le l \le n - 1$, $-l \le m_l \le +l$, $m_s = \pm 1/2$).

3. **Visualizador Interactivo de Orbitales (SVG dinámico):**
   - Representación geométrica de orbitales $s$ (esférico), $p$ ($p_x, p_y, p_z$), $d$ con sus 5 configuraciones diferenciadas (incluyendo $d_{z^2}$ con toroide ecuatorial, $d_{x^2-y^2}$, $d_{xy}$, $d_{xz}$, $d_{yz}$) y $f$.
   - Indicador de planos nodales y fases de la función de onda ($+/-$).
   - Cálculo en vivo de la regla de Madelung $(n + l)$, capacidad del subnivel $2(2l + 1)$ y capacidad del nivel $2n^2$.

4. **Guía Teórica Integrada (PAU):**
   - Fundamentos del modelo mecanocuántico (ecuación de Schrödinger, concepto de orbital con $P > 90\%$).
   - Principios rectores: **Exclusión de Pauli**, **Principio de Aufbau** y **Regla de Hund**.
   - Protocolo oficial de redacción para garantizar la máxima calificación en los exámenes.

5. **Herramientas de Aula y Evaluación Formativa:**
   - **Cronómetro de sesión:** Permite monitorizar el tiempo de trabajo autónomo.
   - **Contador de rachas:** Mantiene la motivación premiando secuencias de aciertos consecutivos.
   - **Informe descargable en PDF:** Generador de actas de sesión con nombre de estudiante, tiempo invertido, aciertos, fallos y auditoría pregunta por pregunta.

6. **Bilingüe e Inclusivo:**
   - Conmutador instantáneo entre **Castellano** y **Catalán** en cabecera sin recargar la página.

---

## 🚀 Despliegue Inmediato en GitHub Pages

La aplicación está contenida en un único archivo auto-suficiente (`index.html`) que no requiere compilación previa (`build`), `npm` ni librerías locales:

1. Crea un repositorio público en tu cuenta de GitHub (por ejemplo, `quimica-cuanticlab`).
2. Sube el archivo `index.html` en la raíz (`root`) del repositorio.
3. En GitHub, accede a **Settings** > **Pages**.
4. En **Build and deployment** > **Branch**, selecciona `main` (o `master`) y la carpeta `/ (root)`. Pulsa **Save**.
5. Tras unos segundos, tu aplicación estará disponible públicamente en:
   
```text
   https://<tu-usuario>.github.io/<nombre-repositorio>/
