# Análisis de Ensayo de Compresión de Hormigón

## 1. Propósito del Proyecto
Este repositorio funciona como un manual de instrucciones para comprender rápidamente la estructura y los problemas del conjunto de archivos originales heredados[cite: 9]. El objetivo es documentar el procedimiento exacto de procesamiento de datos y los supuestos aplicados, separando claramente los archivos de análisis de los de resultados para permitir la reproducibilidad del trabajo[cite: 9].

## 2. Estructura de Carpetas
Para evitar modificaciones accidentales y mejorar la trazabilidad, los archivos se organizaron de la siguiente manera:
* `/datos de origen`: Contiene el registro bruto inalterado del ensayo (`ensayo_hormigon.xlsx`).
* `/análisisprocesos`: Contiene la planilla donde se procesaron los cálculos (`ensayo_hormigon_FINAL_v2.xlsx`).
* `/figurasresultados`: Contiene el gráfico final exportado (`grafico_final.png`).
* `/documentación`: Almacena el informe original (`informe_final.docx`), los apuntes heredados (`notas.txt`) y la plantilla de declaración de IA (`USO_IA_sin_completar.md`).

## 3. Unidades y Supuestos Geométricos
Los archivos originales omitían información vital sobre las magnitudes[cite: 9]. Para interpretar los datos entregados y evitar errores, se establecen los siguientes parámetros:
* **Dimensiones de la probeta:** Diámetro (D) = 150 mm, Altura (H) = 300 mm[cite: 9].
* **Área Transversal:** Para dividir la carga y obtener el esfuerzo, se aplicó la fórmula del área circular: A = π * (D/2)²[cite: 9].
* **Unidades asumidas:** 
  * Desplazamiento (Eje X): mm
  * Esfuerzo (Eje Y): MPa

## 4. Procedimiento de Análisis
El flujo de trabajo que conecta los archivos es el siguiente:
1. Se extrajeron los datos desde el archivo inalterado en `/datos de origen`.
2. Las fórmulas y cálculos intermedios se realizaron en la planilla de Excel ubicada en la carpeta de `/análisisprocesos`[cite: 9].
3. A partir de esos cálculos, se generó la curva final que se encuentra exportada en la carpeta `/figurasresultados`.

## 5. Limitaciones Conocidas (Auditoría Técnica)
Durante la revisión del proyecto se detectaron problemas que no pueden ser resueltos y que afectan la trazabilidad completa del ensayo:
* **Falta de contexto de origen:** No existe información sobre las características del ensayo[cite: 9]. Se desconoce la fecha de ejecución, el tipo de curado, la edad del hormigón, el equipo utilizado y las condiciones del laboratorio, lo que imposibilita analizar la coherencia física de los datos[cite: 9].
* **Uso de IA no verificable:** El informe original indica que se utilizó inteligencia artificial para redactar partes del texto, pero no se registraron los fragmentos generados[cite: 9]. Al no poder contactar al ingeniero original para consultar cómo usó la herramienta, no es posible completar fehacientemente el archivo `USO_IA_sin_completar.md` ni verificar dicho contenido[cite: 9].
## 6. Uso de IA
Herramienta: Gemini (Google)
Propósito: Asistencia para estructurar el archivo README, organizar las carpetas del repositorio y revisar la redacción de la bitácora de auditoría.
Salida utilizada: Propuestas de formato Markdown para el README y retroalimentación sobre la claridad de los problemas detectados.
Cómo se verificó: Se contrastaron las sugerencias con la pauta de evaluación y se adaptaron las respuestas para que reflejaran fielmente los hallazgos personales sobre el proyecto heredado.
Decisión final: Se incorporó la estructura sugerida en el README y en la redacción final de la bitácora. Sobre el uso de IA del autor original, se dejó constancia en el README que es imposible de auditar.