# abm-pedestrian-moral-disengagement
Proyecto abm-pedestrian-moral-disengagement
Modelado Basado en Agentes (ABM) del Flujo Peatonal integrando Desconexión Moral

Este repositorio contiene el código fuente, datos y documentación para el proyecto de investigación: "Impacto de la Desconexión Moral en la seguridad vial: Un enfoque de simulación ABM en intersecciones críticas".

🎯 Objetivo del Proyecto

El objetivo es simular cómo los mecanismos cognitivos de Desconexión Moral (justificación de conductas transgresoras) influyen en la toma de decisiones de los peatones al cruzar intersecciones semaforizadas, generando patrones emergentes de riesgo y accidentalidad.

La Lógica del Modelo (P+V+C)

Propuesta (P): Un modelo de simulación basado en agentes (construido en Python/Mesa).

Valor (V): Cuantificar el incremento en la tasa de incidentes viales y la reducción de la eficiencia del flujo.

Contexto (C): Intersecciones urbanas críticas de alta densidad (ej. Lima Metropolitana).

🧠 La Variable: Desconexión Moral (DM)

A diferencia de los modelos tradicionales de fuerza social (Helbing), este modelo dota a cada agente de un atributo psicosocial moral_disengagement_level (0.0 a 1.0).

Este atributo modifica el umbral de riesgo del agente:

Agentes Normativos (DM Baja): Solo cruzan en verde o cuando la brecha de seguridad es > 5 segundos.

Agentes Transgresores (DM Alta): Tienen probabilidad de cruzar en rojo si:

No perciben coches cercanos (Evaluación de riesgo distorsionada).

Observan a otros cruzando (Efecto rebaño / Difusión de responsabilidad).

📂 Estructura del Repositorio

/models: Contiene la lógica de los agentes (agents.py) y el entorno (model.py).

/data: Contiene las distribuciones estadísticas obtenidas de la validación de la Escala de Desconexión Moral.

/analysis: Jupyter Notebooks para el análisis de sensibilidad y validación de resultados.

🚀 Instalación y Uso

Clonar el repositorio:

git clone [https://github.com/tu-usuario/abm-pedestrian-moral.git](https://github.com/tu-usuario/abm-pedestrian-moral.git)
cd abm-pedestrian-moral


Instalar dependencias:

pip install -r requirements.txt


Ejecutar la simulación:

python run_model.py


📊 Protocolo ODD

La descripción detallada del modelo sigue el protocolo estándar ODD (Overview, Design concepts, Details) y se encuentra disponible en docs/ODD_Protocol.md.

🤝 Contribución

Este proyecto es parte del Grupo de Investigación en Sistemas Complejos de USIL. Las contribuciones son bienvenidas mediante Pull Requests.

📝 Cita

Si utilizas este modelo, por favor cita:

Figueroa-Tejada, G., et al. (2026). Pedestrian moral disengagement scale towards sustainable urban planning. Transportation Research Interdisciplinary Perspectives.

Investigadora Principal: Dra. Gisella Figueroa Tejada
