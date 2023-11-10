# Seminario 4: Mundos virtuales. Introducción a la programación de gráficos 3D - (2)
# Interfaces Inteligentes. Curso 2023 - 2024

## Grupo 4
> Laura Ramallo Pérez
> 
> Adrián Sanz Fernández
> 
> Helena García Díaz

### 1. Investiga sobre los modelo de iluminación que aplica Unity y resume las relaciones existentes con el modelo explicado en clase.

- **Iluminación Local**:
Es el cálculo simple de la luz que afecta directamente a un objeto desde fuentes de luz específicas, sin tener en cuenta la luz que se refleja de otros objetos. Se centra en la luz directa y las sombras que esta crea.

- **Iluminación Global**:
Este modelo tiene en cuenta no solo la luz directa de las fuentes de luz, sino también cómo esa luz se refleja y difunde a través de las superficies de toda la escena, aportando más realismo debido a la inclusión de luz indirecta.

- **Radiosidad**:
Es un método para simular la iluminación global que se enfoca en cómo la luz se dispersa y refleja de manera uniforme en las superficies, considerando la interacción detallada entre la luz y los objetos, lo cual es computacionalmente intensivo y generalmente se precalcula.

- **Iluminación ambiental**:
Para la iluminación ambiental en Unity, no se utilizan luces directas. En cambio, se configura la iluminación ambiental mediante el componente "Skybox" y el entorno de la escena. El "Skybox" envuelve la escena con una textura que proporciona una apariencia general de iluminación ambiental. 

- **Iluminación difusa**:
La iluminación difusa en Unity se logra principalmente utilizando luces como "Point Lights" y "Spot Lights". Estas luces emiten luz en todas direcciones desde un punto o en una dirección específica y afectan a los objetos en la escena.

- **Iluminación especular**:
Para lograr la iluminación especular en Unity, también se utilizan luces como "Point Lights" y "Spot Lights". Además, se pueden emplear cubemaps para simular la reflexión especular en objetos. La configuración de la intensidad de las luces, junto con los mapas de reflexión especular en los materiales de los objetos, permite reflejar la luz de manera más intensa en áreas específicas y direcciones, creando así efectos de brillo y reflejos en las superficies.

### 2. Indica las funciones de la API de Unity más importantes respecto a la iluminación.

- **Light**: La clase `Light` es fundamental en la iluminación de Unity. Se puede utilizar para crear fuentes de luz, como luces direccional, puntual, de punto y área.

- **Lighting**: El sistema de iluminación global (GI) de Unity se puede controlar a través de la API de `Lighting`. Esto incluye el cálculo y la generación de mapas de iluminación global y la gestión de los parámetros relacionados con la GI.

- **Shaders**: Unity ofrece una variedad de shaders integrados que te permiten controlar cómo los objetos reaccionan a la luz. Puedes manipular las propiedades de los materiales, como el brillo, la reflectividad y las sombras, a través de la API de shaders.

- **RenderSettings**: La clase `RenderSettings` permite controlar la configuración global de la iluminación en la escena. Se puede establecer el ambiente y el color de fondo, así como configurar el sistema de iluminación en tiempo real y la iluminación global.

- **Light Probes**: Se puede utilizar `LightProbes` para definir volúmenes de sondas de luz en la escena, lo que te permite mejorar la iluminación de objetos en tiempo real y reflejar la iluminación en objetos estáticos, logrando una mayor coherencia en la escena.

- **Reflection Probes**: Con las clases `ReflectionProbe` y `ReflectionProbeUsage`, se puede configurar y controlar las sondas de reflexión para capturar y aplicar reflexiones en tiempo real en objetos y superficies.

- **Lightmaps**: La API de Unity proporciona funcionalidad para generar y aplicar lightmaps a objetos estáticos en una escena, lo que mejora significativamente la calidad de la iluminación global.

- **Shadows**: Se puede controlar la generación y la calidad de las sombras arrojadas por las luces utilizando la API de sombras, que incluye propiedades como la distancia de sombra, la resolución y el mapeo de sombras.

- **Post-processing Stack**: La API relacionada con el post-procesamiento permite aplicar efectos de post-procesamiento, como corrección de color, desenfoque y efectos de iluminación, para mejorar la calidad visual de tus escenas.

- **Volumentric Lighting**: Se trata de una herramienta para configurar y ajustr efectos de ilumincación volumétrica, lo que permite simular efectos realistas de luz que se dispersa a través de medios como el humo, la niebla o el polvo. 
