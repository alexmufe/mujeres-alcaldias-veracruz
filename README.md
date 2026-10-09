# Mujeres en las alcaldías de Veracruz

## Pregunta

¿Qué diferencias hay entre las candidaturas de mujeres y hombres a las presidencias municipales de Veracruz y cuánto persisten al comparar candidaturas del mismo municipio y partido y ajustar por características observadas? El notebook conserva las especificaciones de los modelos del análisis.

## Fuentes de datos

Los tres CSV incluidos contienen la base de candidaturas, la integración de cargos electos y los indicadores municipales derivados. Las fuentes declaradas para su construcción son el [INE (Conóceles y SICEE)](https://ine.mx/), el [OPLE Veracruz](https://www.oplever.org.mx/) —incluidos cómputos y PREP— y el [Censo de Población y Vivienda 2020 de INEGI](https://www.inegi.org.mx/programas/ccpv/2020/). Consulta de los portales: 9 de octubre de 2026. Los archivos procesados necesarios para reproducir las tablas y modelos están versionados junto al notebook; no hace falta volver a bajar los materiales fuente.

## Cómo reproducirlo

Clona `https://github.com/alexmufe/mujeres-alcaldias-veracruz.git`, entra al directorio, crea un entorno de Python e instala `requirements.txt` con `python -m pip install -r requirements.txt`. Ejecuta todas las celdas de [`Anexo_metodologico_Veracruz_2025.ipynb`](Anexo_metodologico_Veracruz_2025.ipynb) en Jupyter/VS Code, o desde la raíz con `python -m nbconvert --to notebook --execute --inplace --ExecutePreprocessor.timeout=1800 Anexo_metodologico_Veracruz_2025.ipynb`. No se requiere acceso a Colab, rutas locales personales ni descargas.

## Qué produce

El cuaderno genera cuadros de resultados, análisis por subgrupos y gráficas de brechas. Con los datos incluidos reproduce 54 de 212 presidencias municipales ganadas por mujeres, una brecha de 18 puntos con efectos fijos de municipio y partido y de 16 puntos con controles de perfil y antecedentes. Las brechas por subgrupo son 21 y 12 puntos según cargo previo, 24 y 14 según licenciatura, y 24, 15 y 10 por tamaño municipal. La gráfica 2B calcula las tasas por tercil de fuerza del partido y sexo.

## Límites

El análisis es observacional y no identifica efectos causales; las bases no miden recursos de campaña ni apoyo territorial. Las características de perfil dependen de lo declarado en Conóceles y los indicadores censales corresponden a 2020. Los CSV del repositorio son los insumos procesados para reproducir el análisis, no todos los archivos originales de cada institución. El PDF del documento principal no está incluido.
