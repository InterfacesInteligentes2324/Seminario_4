# Seminario 4: Mundos virtuales. Introducción a la programación de gráficos 3D - (2)
# Interfaces Inteligentes. Curso 2023 - 2024

## Grupo 4
> Laura Ramallo Pérez
> 
> Adrián Sanz Fernández
> 
> Helena García Díaz

### 1. Investiga sobre los modelo de iluminación que aplica Unity y resume las relaciones existentes con el modelo explicado en clase.

### 2. Indica las funciones de la API de Unity más importantes respecto a la iluminación.

- **Light**: La clase `Light` es fundamental en la iluminación de Unity. Se puede utilizar para crear fuentes de luz, como luces direccional, puntual, de punto y área.

- **Lighting**: El sistema de iluminación global (GI) de Unity se puede controlar a través de la API de `Lighting`. Esto incluye el cálculo y la generación de mapas de iluminación global y la gestión de los parámetros relacionados con la GI.

- **Shaders**: Unity ofrece una variedad de shaders integrados que te permiten controlar cómo los objetos reaccionan a la luz. Puedes manipular las propiedades de los materiales, como el brillo, la reflectividad y las sombras, a través de la API de shaders.

- **RenderSettings**: La clase `RenderSettings` permite controlar la configuración global de la iluminación en la escena. Se puede establecer el ambiente y el color de fondo, así como configurar el sistema de iluminación en tiempo real y la iluminación global.

- **Light Probes**: Se puede utilizar `LightProbes` para definir volúmenes de sondas de luz en la escena, lo que te permite mejorar la iluminación de objetos en tiempo real y reflejar la iluminación en objetos estáticos.

- **Reflection Probes**: Con las clases `ReflectionProbe` y `ReflectionProbeUsage`, se puede configurar y controlar las sondas de reflexión para capturar y aplicar reflexiones en tiempo real en objetos y superficies.

- **Lightmaps**: La API de Unity proporciona funcionalidad para generar y aplicar lightmaps a objetos estáticos en una escena, lo que mejora significativamente la calidad de la iluminación global.

- **Shadows**: Se puede controlar la generación y la calidad de las sombras arrojadas por las luces utilizando la API de sombras, que incluye propiedades como la distancia de sombra, la resolución y el mapeo de sombras.

- **Post-processing Stack**: La API relacionada con el post-procesamiento permite aplicar efectos de post-procesamiento, como corrección de color, desenfoque y efectos de iluminación, para mejorar la calidad visual de tus escenas.
