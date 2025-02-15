# Sistema IoT para Detección de Incendios en los Cerros Orientales de Bogotá - Challenge 1

## 1. Introducción
<p align="justify">
Los cerros orientales de Bogotá son fundamentales para la regulación climática y la conservación de la biodiversidad. Su presencia como barrera y protector natural constituye un regulador del clima, del cual depende en buena medida la disponibilidad de agua para la capital y municipios aledaños [1]. Además, son esenciales en la producción de oxígeno en una sabana donde la pérdida de vegetación es creciente, lo que los hace aún más vulnerables a incendios forestales agravados por sequías prolongadas, altas temperaturas y la acumulación de material seco, junto con actividades humanas como fogatas, quemas agrícolas y expansión urbana descontrolada [2]. Un aumento repentino de temperatura, junto con la detección de llamas y gases como CO y CO₂, son indicadores claves de incendios. Implementar una solución basada en Internet de las Cosas que analice estos datos permitirá un monitoreo continuo y alertas tempranas, reduciendo la propagación del fuego y sus impactos negativos.
</p>

### Motivación y Justificación
<p align="justify">
Actualmente, la detección de incendios en los cerros orientales de Bogotá depende de vigilancia manual o reportes ciudadanos, lo que retrasa la respuesta de las autoridades y agrava los daños ambientales y sociales. La implementación de un sistema basado en Internet de las Cosas permitirá una monitorización continua y la activación inmediata de alarmas visuales y sonoras, facilitando una intervención más rápida y eficiente ante posibles incendios forestales.  
</p>
<p align="justify">
Este proyecto integra un DS18B20, un sensor de llama y un MQ-2, los cuales detectan variaciones en temperatura, presencia de fuego y concentración de gases inflamables. La información recopilada es procesada por un Arduino Uno R3, que gestiona la activación de alertas mediante un zumbador activo, un LED RGB y un módulo LCD I2C para notificaciones en tiempo real. Gracias a su diseño compacto y autónomo, el sistema puede operar en entornos remotos sin depender de redes externas, lo que lo hace ideal para zonas con infraestructura de comunicación limitada.Con esta solución, se busca optimizar los tiempos de respuesta, reducir el impacto ambiental de los incendios y fortalecer las estrategias de prevención.
</p>

### Estructura de la Documentación
<p align="justify">
La documentación se organiza en las siguientes secciones:
</p>

#### **2. Solución Propuesta**
<p align="justify">
Se describen las restricciones de diseño, la arquitectura del sistema mediante un diagrama de bloques y el desarrollo modular de la solución, incluyendo diagramas UML y esquemáticos de hardware.
</p>

#### **3. Configuración Experimental, Resultados y Análisis**
<p align="justify">
Se detallan las pruebas realizadas para validar el funcionamiento del sistema, la evaluación del desempeño en diferentes condiciones ambientales y el análisis de los resultados obtenidos en comparación con las expectativas iniciales.
</p>

#### **4. Autoevaluación del Protocolo de Pruebas**
<p align="justify">
Se evalúa la robustez del sistema frente a diferentes escenarios, se identifican mejoras en la metodología de pruebas y se analizan los aspectos críticos del protocolo de pruebas aplicado.
</p>

#### **5. Conclusiones, Retos y Trabajo Futuro**
<p align="justify">
Se presentan los logros alcanzados, los desafíos encontrados durante el desarrollo del proyecto y las posibles mejoras para futuras implementaciones y escalabilidad del sistema.
</p>

#### **6. Referencias**
<p align="justify">
Se listan las fuentes utilizadas en la investigación y desarrollo del sistema y del presente articulo.
</p>

#### **7. Anexos**
<p align="justify">
Incluye el código fuente documentado, los esquemáticos eléctricos y PCB, así como material complementario relevante para la comprensión del proyecto.
</p>

## 2. Solución Propuesta

## 3. Configuración Experimental, Resultados y Análisis

## 4. Evaluación del Protocolo de Pruebas
- Evaluación de la robustez del sistema frente a diferentes condiciones ambientales.
- Identificación de mejoras en el proceso de pruebas.
- Comparación de desempeño con expectativas iniciales.

## 5. Conclusiones, Retos y Mejoras Futuras

## 6. Referencias
[1] N. Bustamante, “La importancia de proteger a los cerros orientales de Bogotá,” *El Tiempo*, 26 de febrero de 2019. [Online]. Disponible en: [https://www.eltiempo.com/vida/ciencia/la-importancia-de-proteger-a-los-cerros-orientales-de-bogota-279294](https://www.eltiempo.com/vida/ciencia/la-importancia-de-proteger-a-los-cerros-orientales-de-bogota-279294). [Accedido: 12-feb-2025].  

[2] El Espectador, “Incendio forestal en los cerros orientales de Bogotá: ¿Por qué se producen?,” *El Espectador*, 31 de enero de 2023. [Online]. Disponible en: [https://www.elespectador.com/cromos/famosos/incendio-forestal-en-los-cerros-orientales-de-bogota-por-que-se-producen/](https://www.elespectador.com/cromos/famosos/incendio-forestal-en-los-cerros-orientales-de-bogota-por-que-se-producen/). [Accedido: 12-feb-2025].  

## 7. Anexos

```

