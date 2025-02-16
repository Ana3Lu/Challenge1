# Sistema IoT para Detección de Incendios en los Cerros Orientales de Bogotá - Challenge 1

## Información del Proyecto
- **Universidad:** Universidad de La Sabana  
- **Facultad:** Facultad de Ingeniería  
- **Materia:** Internet de las Cosas  
- **Profesor:** Juan Manuel Aranda López King  

## Integrantes del Proyecto
| Nombre | Correo Electrónico |
|--------|-------------------|
| Mariana Valle Moreno | marianavamo@unisabana.edu.co |
| Valentina Alejandra López Romero | valentinalopro@unisabana.edu.co |
| [Nombre 3] | [correo3@ejemplo.com] |

## Estructura de la Documentación
- [1. Introducción](#1-introducción)
- [2. Motivación y Justificación](#2-motivación-y-justificación)
- [3. Solución Propuesta](#3-solución-propuesta)
- [4. Configuración Experimental, Resultados y Análisis](#4-configuración-experimental-resultados-y-análisis)
- [5. Autoevaluación del Protocolo de Pruebas](#5-autoevaluación-del-protocolo-de-pruebas)
- [6. Conclusiones, Retos y Mejoras Futuras](#6-conclusiones-retos-y-mejoras-futuras)
- [7. Referencias](#7-referencias)
- [8. Anexos](#8-anexos)

---

## 1. Introducción
<p align="justify">
Los cerros orientales de Bogotá son fundamentales para la regulación climática y la conservación de la biodiversidad. Su presencia como barrera y protector natural constituye un regulador del clima, del cual depende en buena medida la disponibilidad de agua para la capital y municipios aledaños [1]. Además, son esenciales en la producción de oxígeno en una sabana donde la pérdida de vegetación es creciente, lo que los hace aún más vulnerables a incendios forestales agravados por sequías prolongadas, altas temperaturas y la acumulación de material seco, junto con actividades humanas como fogatas, quemas agrícolas y expansión urbana descontrolada [2]. Un aumento repentino de temperatura, junto con la detección de llamas y gases como CO y CO₂, son indicadores clave de incendios. Implementar una solución basada en Internet de las Cosas que analice estos datos permitirá un monitoreo continuo y alertas tempranas, reduciendo la propagación del fuego y sus impactos negativos.
</p>

---

## 2. Motivación y Justificación
<p align="justify">
Actualmente, la detección de incendios en los cerros orientales de Bogotá depende de vigilancia manual o reportes ciudadanos, lo que retrasa la respuesta de las autoridades y agrava los daños ambientales y sociales. La implementación de un sistema basado en Internet de las Cosas permite el monitoreo continuo y la activación inmediata de alarmas visuales y sonoras, facilitando una intervención más rápida y eficiente ante posibles incendios forestales.  
</p>
<p align="justify">
Este proyecto integra un DS18B20, un sensor de llama y un MQ-2, los cuales detectan variaciones en temperatura, presencia de fuego y concentración de gases inflamables. La información recopilada es procesada por un Arduino Uno R3, que gestiona la activación de alertas mediante actuadores como un zumbador activo, un LED RGB y un módulo LCD I2C para notificaciones en tiempo real. Gracias a su diseño compacto y autónomo, el sistema puede operar en entornos remotos sin depender de redes externas, lo que lo hace ideal para zonas con infraestructura de comunicación limitada. Esta solución busca optimizar los tiempos de respuesta, reducir el impacto ambiental de los incendios y fortalecer las estrategias de prevención.
</p>

---

## 3. Solución Propuesta

***Restricciones de Diseño Identificadas***

El diseño del sistema IoT para la detección de incendios en los cerros orientales de Bogotá está sujeto a diversas restricciones que afectan su implementación. Estas restricciones se clasifican en diferentes categorías:

1. **Técnicas**  
   - Uso de un **Arduino Uno R3**, que tiene limitaciones de procesamiento y memoria, restringiendo la cantidad de sensores y el tipo de algoritmos que se pueden ejecutar.  
   - Los sensores seleccionados (DS18B20, MQ-2 y sensor de llama) tienen rangos de medición específicos y requieren calibración para minimizar falsos positivos.  
   - La alimentación debe ser autónoma (baterías o panel solar) para operar en zonas sin acceso a la red eléctrica.  

2. **Económicas**  
   - Se busca minimizar costos utilizando componentes accesibles y ampliamente disponibles en el mercado.  
   - Se prioriza el uso de sensores de bajo costo en lugar de tecnologías más avanzadas (como cámaras térmicas).  

3. **Regulatorias**  
   - El dispositivo debe cumplir con las normativas ambientales y de seguridad eléctrica para su implementación en áreas naturales protegidas.  
   - La instalación de equipos en los cerros debe alinearse con regulaciones locales de conservación ambiental.  

4. **Espaciales**  
   - El sistema debe ser compacto y resistente a condiciones ambientales adversas (lluvia, humedad y polvo).  
   - Se debe considerar la ubicación estratégica de los sensores para maximizar la detección sin afectar la fauna o flora del área.  

5. **Escalabilidad**  
   - Aunque el prototipo se diseña para una zona específica, debe permitir la integración con sistemas más grandes en caso de futuras expansiones.  
   - Se contempla la posibilidad de agregar más sensores en versiones futuras.  

6. **Temporales**  
   - El sistema debe procesar datos en tiempo real para garantizar una detección oportuna.  
   - La autonomía del sistema debe permitir su funcionamiento continuo sin intervención frecuente para mantenimiento.  


***Estándares de Ingeniería Aplicados***

Para garantizar la calidad, seguridad y efectividad del sistema, se han aplicado los siguientes estándares de ingeniería:

1. **Normas de Sensores y Electrónica**  
   - **IEEE 1451**: Define estándares para la interoperabilidad de sensores y dispositivos de medición en sistemas IoT.  
   - **ISO 9001**: Se sigue un enfoque estructurado de desarrollo para asegurar la calidad del diseño y la fabricación del prototipo.  

2. **Seguridad y Medio Ambiente**  
   - **ISO 14001**: Consideraciones ambientales en el diseño y operación del sistema para minimizar el impacto ecológico.  
   - **IEC 60529 (IP Rating)**: Evaluación de la resistencia a polvo y agua para la protección del hardware en exteriores.  

3. **Protocolos de Diseño Electrónico**  
   - **IPC-2221**: Normativa para el diseño de circuitos electrónicos, asegurando la confiabilidad y seguridad del hardware.  
   - **IEC 61000-4-2**: Protección contra descargas electrostáticas en entornos donde pueda haber interferencias electromagnéticas.  

4. **Estándares de Programación y Software**  
   - **ISO/IEC 25010**: Estándar para evaluar la calidad del software en términos de desempeño, confiabilidad y mantenibilidad.  
   - **Arduino Coding Standards**: Buenas prácticas para la programación en C/C++ en microcontroladores Arduino.  


***Desarrollo Teórico Modular: Criterios de Diseño Establecidos***

Para garantizar un diseño eficiente y funcional, se han definido los siguientes criterios de diseño:

1. **Fiabilidad y Precisión**  
   - Selección de sensores con alta sensibilidad y precisión en la detección de temperatura, gases y llamas.  
   - Implementación de algoritmos de calibración y filtrado de datos para minimizar falsas alarmas.  

2. **Bajo Consumo Energético**  
   - Uso de componentes de bajo consumo energético para prolongar la vida útil de la batería.  
   - Implementación de modos de bajo consumo en el microcontrolador para optimizar la energía.  

3. **Autonomía y Mantenimiento Reducido**  
   - Sistema autónomo que no requiere conexión a redes externas para operar.  
   - Diseño resistente a condiciones ambientales adversas para minimizar la necesidad de mantenimiento frecuente.  

4. **Interfaz de Usuario Intuitiva**  
   - Uso de un LCD I2C para visualización clara de los datos en tiempo real.  
   - Incorporación de alarmas visuales (LED RGB) y sonoras (zumbador activo) para alertas inmediatas.  

5. **Escalabilidad y Modularidad**  
   - Diseño modular que permite la integración de nuevos sensores o mejoras en futuras versiones.  
   - Posibilidad de adaptación para conectividad remota en versiones futuras sin modificar la arquitectura base del sistema.

---

## 4. Configuración Experimental, Resultados y Análisis

---

## 5. Autoevaluación del Protocolo de Pruebas

- Evaluación de la robustez del sistema frente a diferentes condiciones ambientales.
- Identificación de mejoras en el proceso de pruebas.
- Comparación de desempeño con expectativas iniciales.

---

## 6. Conclusiones, Retos y Mejoras Futuras

---

## 7. Referencias

[1] N. Bustamante, “La importancia de proteger a los cerros orientales de Bogotá,” *El Tiempo*, 26 de febrero de 2019. [Online]. Disponible en: [https://www.eltiempo.com/vida/ciencia/la-importancia-de-proteger-a-los-cerros-orientales-de-bogota-279294](https://www.eltiempo.com/vida/ciencia/la-importancia-de-proteger-a-los-cerros-orientales-de-bogota-279294). [Accedido: 12-feb-2025].  

[2] El Espectador, “Incendio forestal en los cerros orientales de Bogotá: ¿Por qué se producen?,” *El Espectador*, 31 de enero de 2023. [Online]. Disponible en: [https://www.elespectador.com/cromos/famosos/incendio-forestal-en-los-cerros-orientales-de-bogota-por-que-se-producen/](https://www.elespectador.com/cromos/famosos/incendio-forestal-en-los-cerros-orientales-de-bogota-por-que-se-producen/). [Accedido: 12-feb-2025].  

---

## 8. Anexos

```

