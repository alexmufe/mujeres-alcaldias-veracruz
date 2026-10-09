# Mujeres en las alcaldías de Veracruz

## Pregunta

¿Por qué, aunque la mitad de las candidaturas a presidencias municipales en Veracruz son mujeres, ellas reciben menos votos y ganan menos alcaldías?

## Fuentes de datos

Los CSV incluidos contienen los insumos procesados a partir de [INE (Conóceles y SICEE)](https://ine.mx/), [OPLE Veracruz](https://www.oplever.org.mx/) —incluidos los cómputos y el PREP extraordinario de Tamiahua— y el [Censo de Población y Vivienda 2020 de INEGI](https://www.inegi.org.mx/programas/ccpv/2020/). Los datos electorales y de integración cubren 2021 y 2025; la base incluye la elección extraordinaria de Tamiahua de marzo de 2026. Consulta de los portales: 9 de octubre de 2026.

## Cómo reproducirlo

Clona `https://github.com/alexmufe/mujeres-alcaldias-veracruz.git`, instala las versiones fijadas con `python -m pip install -r requirements.txt` y ejecuta todas las celdas de [`Anexo_metodologico_Veracruz_2025.ipynb`](Anexo_metodologico_Veracruz_2025.ipynb). Para correrlo desde la raíz con un kernel nuevo: `python -m nbconvert --to notebook --execute --inplace --ExecutePreprocessor.timeout=1800 Anexo_metodologico_Veracruz_2025.ipynb`. Los CSV están incluidos y no se necesitan descargas.

## Qué produce

El notebook reproduce 54 de 212 presidencias ganadas por mujeres, una brecha de 18 puntos frente a candidatos de la misma elección y partido y de 16 puntos con controles de perfil y antecedentes. Las brechas son 21 y 12 puntos según experiencia previa en cargos públicos, 24 y 14 según licenciatura, y 24, 15 y 10 por tamaño municipal. En la gráfica 2B, las tasas de victoria de candidatas y candidatos, respectivamente, son 7% y 24% en fuerza débil, 5% y 24% en fuerza media, y 19% y 37% en fuerza fuerte. Se pueden consultar las [gráficas 1A](docs/figuras/grafica_1A_participacion.png), [1B](docs/figuras/grafica_1B_brechas.png) y [2A–2B](docs/figuras/grafica_2_fuerza_partido.png).

## Límites

La brecha de votos no se explica solo por dónde compiten las mujeres: el análisis reporta que persiste frente a candidaturas de la misma elección y frente a perfiles equivalentes. La relevancia de las propuestas no muestra un efecto estadísticamente significativo sobre el voto (1.2 puntos; p = 0.41). El apellido compartido con una autoridad saliente no demuestra parentesco. Las cifras sobre parentesco y algunos resultados legislativos citados en el documento provienen de fuentes externas, no de los CSV que permiten correr el notebook.

**Documento completo:** [Análisis de las candidaturas a las alcaldías de Veracruz](docs/Mujeres_alcaldias_Veracruz_AlejandroMunoz.md).
