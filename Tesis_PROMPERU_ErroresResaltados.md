
	





Universidad Nacional Mayor de San Marcos
Universidad del Perú. Decana de América

Dirección General de Estudios de Posgrado
Facultad de Ingeniería de Sistemas e Informática
Unidad de Posgrado


Framework Basado en IA para estandarizar el proceso de migración de aplicaciones web en entidades públicas: Caso PROMPERU

TESIS
Para optar el Grado Académico de Magíster en Ingeniería de Sistemas e Informática con mención en Ingeniería de Software


AUTOR
Ronald Alexander GUILLERMO NAVARRO


ASESOR
xxxx


Lima, Perú

xx





PLANTEAMIENTO DEL PROBLEMA

Situación Problemática

Hoy en día las instituciones públicas están pasando por un proceso de transformación digital, cuyo fin es brindar un mejor servicio al ciudadano a través de la digitalización de servicios que permita optimizar los procesos, tanto así que la importancia de contar con herramientas tecnológicas que respondan a las necesidades del ciudadano sean una prioridad.

En el sector público peruano, las aplicaciones web institucionales suelen estar alojados en infraestructuras contratadas a terceros, como servicios de hosting, alquiler de servidores dedicados (housing) o plataformas en la nube, por periodos administrativos determinados. 

Una vez vencidos dichos periodos, las entidades deben migrar los sistemas a entornos temporales hasta concretar nuevas adjudicaciones. Este proceso genera riesgos técnicos, costos operativos elevados y pérdida de disponibilidad del servicio.

La complejidad y antigüedad de muchos sistemas legados agrava este panorama, extendiendo los tiempos de migración y reduciendo la disponibilidad de los sistemas al ser migrados a nuevos entornos. Asimismo, la carencia de mecanismos de trazabilidad impide a las entidades cumplir con auditorías internas o reportes de control institucional.

El estado peruano en conjunto con el Centro de Cooperación en Gobierno Digital Corea-Perú establecieron en el 2023 una hoja de ruta para la migración de servicios a la nube, estableciendo como fecha de inicio en el año 2025 y terminando en el 2027.




Fig1: Estrategias y Normativas del Estado Peruano
Fuente: Elaboración propia


De acuerdo con lo mencionado, la migración hacia la nube ya no es solo una necesidad sino una obligación por parte de las entidades públicas a fin de cumplir con los lineamientos de la transformación digital.

PROMPERU es una institución del estado encargada de la difusión y promoción de las exportaciones y el turismo, entre las diversas herramientas de difusión utilizadas se encuentran las aplicaciones web, por medio de ellas se publicita una serie de campañas, ferias, eventos y demás actividades relacionadas con la promoción del turismo y las exportaciones.

Muchas de sus aplicaciones web son reconocidas como un medio muy importante para la información de turismo y exportaciones, tales como peru.travel, ytuqueplanes.com, exportemos.pe, turismoin, etc.



Fig2: Reconocimientos a los portales de PROMPERU
Fuente: Peru Travel



Actualmente estas aplicaciones web se encuentran bajo un alojamiento de tipo hosting, el cual está contratado por un periodo de 2 años.



Fig3: Contrato de servicio hosting año 2021, clausula 5
Fuente: PROMPERU


La gestión de múltiples aplicaciones web en PROMPERÚ representa un desafío operativo crítico, especialmente en un entorno donde la presencia digital es fundamental para promover el turismo y las exportaciones peruanas. Sin embargo, la falta de un proceso de migración optimizado y estandarizado genera frecuentes periodos de inaccesibilidad en sus sitios web, lo que conlleva consecuencias negativas en tres niveles clave:

Impacto Institucional

Daña la imagen de modernidad y confiabilidad de PROMPERÚ ante ciudadanos, turistas y empresarios, quienes esperan servicios digitales ágiles y sin interrupciones.

Limitaciones Operativas

Obstaculiza la difusión oportuna de campañas promocionales, eventos internacionales y lanzamientos estratégicos, reduciendo su alcance y efectividad.

Efecto en los Objetivos de la institución

Debilita la capacidad de la institución para atraer inversiones, promover destinos turísticos y dinamizar las exportaciones, aspectos centrales de su mandato como entidad promotora del desarrollo económico.

Ante este escenario, la falta de un sistema institucionalizado y estandarizado para migraciones de aplicaciones en PROMPERÚ obliga a los desarrolladores a implementar soluciones ad hoc, basadas en criterios individuales. Esta carencia de protocolos unificados genera tres riesgos críticos:

Exposición operativa

Aumenta la probabilidad de errores durante las migraciones, ya que cada equipo aplica metodologías dispares sin supervisión técnica centralizada.

Brechas de gobernanza

Dificulta la trazabilidad de los procesos, afectando el cumplimiento de auditorías y estándares de calidad.

Vulnerabilidad institucional

Crea dependencia de conocimientos especializados no documentados, lo que:

Eleva el riesgo ante rotación de personal.

Compromete la continuidad de los servicios digitales al perder expertise clave.

Esta situación no solo impacta la eficiencia técnica, sino que pone en jaque la capacidad de PROMPERÚ para garantizar servicios digitales estables y escalables, fundamentales para su misión promotora.


Formulación del Problema

Problema general

¿De qué manera puede estandarizarse la gestión de la migración de aplicaciones web en entidades públicas peruanas para asegurar la continuidad operativa, minimizar errores y reducir tiempos de implementación?

Problemas específicos

¿De qué manera la ausencia de procedimientos estandarizados de migración afecta la continuidad operativa y la integridad de las aplicaciones web de PROMPERÚ?

¿Cómo influye la dependencia del conocimiento individual del personal técnico en los tiempos y la eficiencia de los procesos de migración de aplicaciones web en PROMPERÚ?

¿Cuáles son los desafíos técnicos específicos que enfrentan las aplicaciones web legadas de PROMPERÚ durante los procesos de migración a nuevos entornos?

¿Cómo impacta la carencia de mecanismos de trazabilidad y monitoreo en la capacidad de PROMPERÚ para auditar y controlar eficazmente el proceso de migración de sus aplicaciones web?


Justificación de la Investigación

Justificación teórica

El vertiginoso avance tecnológico exige que los sistemas actuales se adapten continuamente para mantener su relevancia y eficiencia. En este contexto, la implementación de la Inteligencia Artificial (IA) en los procesos de gestión del software emerge como una estrategia crucial para optimizar la eficiencia y reducir la dependencia de la intervención humana directa. Esto es especialmente relevante en el ámbito de la migración de aplicaciones, un proceso que, como se observa en el sector público peruano y específicamente en PROMPERÚ, es propenso a ineficiencias, errores y largos tiempos de transferencia debido a la ausencia de procesos estandarizados y la dependencia del conocimiento individual.

A pesar de la proliferación de herramientas de gestión de software en el mercado, como ClickUp, AWS CodeDeploy, CircleCI, GitLab, Octopus Deploy, Bamboo, Codeship, Travis CI, Jenkins y Puppet, se identifica una limitación significativa: la carencia de integración con capacidades de IA y de funcionalidades que permitan una transición eficiente entre diferentes entornos. Ninguna de las herramientas mencionadas incorpora explícitamente inteligencia artificial en sus procesos ni ofrece una funcionalidad robusta diseñada específicamente para facilitar la migración de ambientes de producción de forma agnóstica al proveedor. Esta limitación inherente afecta directamente la capacidad de adaptación rápida de las entidades públicas ante cambios de infraestructura y su necesidad imperante de migrar sistemas de un entorno a otro sin interrupciones significativas, un desafío crítico en el contexto de contratos de alojamiento temporales y la inminente migración a la nube establecida para 2025-2027 en Perú.

El estudio y desarrollo de soluciones basadas en IA adquiere una relevancia particular en el escenario actual de las entidades públicas, las cuales están inmersas en un proceso de transformación digital. La integración de la IA en la gestión de TI es un componente estratégico, tal como indica Haidar (2024, p. 5), quien subraya que "la estrategia de uso de IA debe estar enfocada a la estrategia del gobierno de TI, con lo cual aseguramos estar alineados con los objetivos de las entidades públicas". Esta alineación es fundamental para que la optimización de la migración de aplicaciones contribuya directamente a los objetivos de servicio al ciudadano y eficiencia estatal.

Aporte Basado en SWEBOK 4 para la Ingeniería de Software

Desde la perspectiva de la Ingeniería de Software, la gestión de la migración de sistemas no solo implica aspectos técnicos, sino también de proceso y mantenimiento. El Cuerpo de Conocimiento de Ingeniería de Software (SWEBOK 4), en su área de conocimiento de Mantenimiento de Software, destaca la importancia de las actividades de adaptación y reubicación de software. Si bien SWEBOK 4 no aborda explícitamente la IA, sí enfatiza la necesidad de automatización, mejora de procesos y reducción de la complejidad en las tareas de mantenimiento y evolución de sistemas. La migración, al ser una forma compleja de cambio de entorno, se beneficia directamente de principios que buscan minimizar riesgos y asegurar la calidad del software.

El presente estudio, al proponer un framework basado en IA para la migración, contribuye directamente a estas líneas. Busca mejorar la disciplina de la Ingeniería de Software al ofrecer un enfoque innovador para:

Reducir los costos y riesgos asociados con las migraciones, un problema recurrente en el mantenimiento de sistemas legados.

Aumentar la eficiencia y la predictibilidad del proceso de migración a través de la automatización inteligente.

Facilitar la reubicación de sistemas, un concepto crucial para la adaptabilidad de software en entornos cambiantes, como la adopción de la nube.

Este aporte se alinea con la meta de SWEBOK 4 de promover un conocimiento estructurado y práctico que permita a los ingenieros de software abordar desafíos complejos y en evolución, como la gestión de grandes volúmenes de aplicaciones en entornos dinámicos del sector público.




Beneficios de la Optimización de la Migración mediante IA

La aplicación de IA en la gestión de la migración de aplicaciones promete múltiples beneficios que abordan directamente los problemas identificados:

Escalabilidad: Permite el ajuste dinámico de recursos según las necesidades de carga durante y después del proceso de migración.

Mejores tiempos de transferencia: Facilita procesos de migración más rápidos y eficientes, reduciendo la ventana de indisponibilidad del servicio.

Alta disponibilidad: Contribuye a una mayor continuidad en los servicios ofrecidos al minimizar interrupciones durante el traslado.

Posibilidad de balanceo de carga: Ofrece la capacidad de distribuir automáticamente la carga de trabajo, optimizando el rendimiento post-migración.

Minimización de errores en la migración: La IA puede predecir y mitigar fallos, reduciendo los problemas técnicos asociados al proceso.

Reducción de la dependencia de personal: Al automatizar y optimizar tareas complejas de migración, se minimiza la intervención humana, permitiendo que los equipos técnicos se enfoquen en tareas de mayor valor.

Adicionalmente, la presente investigación busca justificar cómo la adopción de la IA en la gestión de la migración de aplicaciones web contribuirá a la eliminación de las dependencias de proveedores, conocidas como "vendor lock-in". De acuerdo con Korontanis, Makris y Tserpes (2024), "la adopción de estrategias para el agnosticismo de los sistemas facilitará la independencia del proveedor, de manera que no tenga interacción directa". Este aspecto es crucial para las entidades públicas que actualmente operan con infraestructuras contratadas por periodos determinados, permitiendo una mayor flexibilidad y resiliencia ante futuros cambios de proveedores o entornos tecnológicos.


Justificación práctica

La presente investigación posee una significativa justificación práctica al abordar un problema operativo crítico que enfrentan actualmente las entidades públicas peruanas, y específicamente PROMPERÚ: la gestión ineficiente y riesgosa de la migración de aplicaciones web. Ante la inminente obligación del Estado peruano de migrar servicios a la nube para 2025-2027 y la problemática recurrente de la dependencia de contratos de alojamiento temporales, la necesidad de una solución efectiva es apremiante.

El desarrollo de un framework basado en inteligencia artificial para la gestión de la migración de aplicaciones web ofrecerá beneficios tangibles y directos:

Para PROMPERÚ:

Mejora de la Continuidad Operativa: El framework permitirá realizar procesos de migración de sus múltiples y críticas páginas web (como peru.travel, ytuqueplanes.com, exportemos.pe) con mínimas interrupciones. Esto es fundamental para asegurar la difusión constante de campañas de turismo y exportaciones, preservando la imagen institucional y evitando la pérdida de oportunidades de negocio e inversión.

Reducción de Tiempos y Costos: Al automatizar y optimizar las actividades de migración mediante IA, se disminuirán significativamente los tiempos de transferencia de ambientes, lo que se traducirá en una reducción de los costos operativos asociados a largos periodos de inactividad o la necesidad de recursos adicionales para resolver incidencias manuales.

Minimización de Errores y Riesgos: La capacidad de la IA para analizar el estado de los ambientes, generar planes precisos y aplicar los cambios con mayor exactitud, reducirá drásticamente la probabilidad de inconsistencias, fallos y otros problemas técnicos durante las migraciones, que actualmente dependen del expertise individual y generan alta exposición operativa.

Eliminación de la Dependencia del Personal y Estandarización: El framework institucionalizará los procedimientos de migración, reduciendo la alta dependencia del conocimiento tácito de desarrolladores específicos. Esto facilitará la estandarización de procesos, mejorará la capacitación de nuevos talentos y asegurará la continuidad operativa frente a la rotación de personal.

Mayor Control y Trazabilidad: La inclusión de mecanismos de trazabilidad en cada actividad de migración permitirá a PROMPERÚ cumplir con requisitos de auditoría interna y reportes de control institucional, mejorando la gobernanza y la transparencia de sus operaciones tecnológicas.

Para el Sector Público Peruano:

Precedente para la Transformación Digital: El éxito de este framework en PROMPERÚ sentará un precedente valioso y ofrecerá un modelo replicable para otras entidades públicas peruanas que enfrentan desafíos similares en su proceso de migración a la nube y transformación digital. Demostrará cómo la aplicación de IA puede ser una herramienta clave para superar barreras técnicas y operativas.

Fomento de la Independencia Tecnológica: Al facilitar el agnosticismo del proveedor en la migración de sistemas, la investigación contribuirá a que las entidades públicas eviten el "vendor lock-in", promoviendo una mayor autonomía en sus decisiones de infraestructura y optimizando la inversión de recursos del Estado a largo plazo.

En síntesis, esta tesis no es solo un aporte teórico, sino una propuesta práctica que busca fortalecer la infraestructura tecnológica de PROMPERÚ, dotándola de una herramienta innovadora y eficiente para gestionar sus migraciones de aplicaciones web, lo cual impactará directamente en su capacidad para cumplir su misión promotora y en la calidad de los servicios digitales que ofrece al ciudadano.


Objetivos de la Investigación

Objetivo General
Desarrollar un framework basado en inteligencia artificial para estandarizar la gestión de la migración de aplicaciones web en entidades públicas peruanas, con un enfoque en PROMPERÚ, con el fin de garantizar la continuidad operativa, reducir los tiempos de transferencia y minimizar los errores durante el proceso de migración.

Objetivos Específicos

Analizar los requisitos funcionales y no funcionales para la gestión de la migración de aplicaciones web en PROMPERÚ, incluyendo la identificación de puntos críticos y dependencias en los ambientes de producción.

Diseñar la arquitectura y los componentes de un framework de gestión de migración de aplicaciones web, que incorpore capacidades de inteligencia artificial para la generación automatizada de planes de migración.

Implementar los módulos clave del framework propuesto que permitan la aplicación automatizada de los planes de migración y la recolección de datos para la trazabilidad.

Evaluar la efectividad del framework propuesto en la optimización de la continuidad operativa, la reducción de los tiempos de transferencia y la minimización de errores durante los procesos de migración de aplicaciones web en un entorno simulado o piloto en PROMPERÚ.

MARCO TEÓRICO

Antecedentes de la Investigación

La optimización de los procesos de software es un desafío constante en el desarrollo de sistemas. Tradicionalmente, la gestión de la migración se ha abordado bajo un concepto de automatización, buscando optimizar la transición de sistemas entre diferentes entornos. Sin embargo, este proceso es inherentemente complejo y dinámico, especialmente en entidades públicas donde los ambientes de producción suelen ser itinerantes debido a ciclos de contratación y evolución tecnológica. En este contexto, resulta de suma importancia establecer un control robusto sobre cada etapa, desde una solicitud de pase a un nuevo ambiente de producción hasta una migración rápida entre infraestructuras.

En ese sentido, se presentan las siguientes investigaciones previas que proporcionan una base sólida para comprender los desafíos y las oportunidades en la gestión de la migración de aplicaciones web con inteligencia artificial:

Factores de éxito en la gestión de proyectos DevOps: Un marco de toma de decisiones. El artículo de Akbar et al. (2023) destaca los factores determinantes para el éxito en proyectos que involucran la automatización y la integración continua de software. Subrayan la importancia de la automatización, la colaboración interdisciplinaria y la integración de herramientas tecnológicas avanzadas para optimizar la evolución continua de software. Aunque enfocado en DevOps, el estudio propone un marco metodológico basado en el PMBOK, complementado con técnicas como Fuzzy-AHP, para abordar retos como la transición de entornos y la mitigación de errores en ambientes de producción. Este enfoque se alinea con la creciente demanda de sistemas inteligentes que faciliten migraciones eficientes y robustas en el sector público.

Inteligencia artificial en la gestión organizacional: Impacto y realidad latinoamericana. Este artículo de Rodríguez-Alegre, L. R., Calderón-De-Los-Ríos, H., Hurtado-Zamora, M. M., & Ocaña-Rodríguez, Á. W. (2023) analiza cómo la IA puede transformar la gestión organizacional en entidades públicas, mejorando la eficiencia en procesos operativos. La investigación discute las implicaciones éticas y la necesidad de regulaciones adecuadas para su implementación efectiva, proporcionando un marco contextual relevante para la adopción de IA en la administración pública peruana para la gestión de la migración.

Operacionalización de Modelos de Aprendizaje Automático: Una Revisión Sistemática de la Literatura. En este artículo, Kolltveit y Li (2022) revisan la integración de machine learning en los ambientes de producción, un tema directamente relacionado con la aplicación de IA en la gestión de la migración que propone esta tesis. Proponen herramientas y técnicas para el empaquetado, integración, y monitoreo de modelos de ML en entornos productivos. Asimismo, identifican desafíos a superar como la necesidad de monitoreo continuo y adaptación a los cambios en los frameworks de IA (TensorFlow, PyTorch, Scikit-learn), lo cual es crucial para mantener actualizado y efectivo un sistema inteligente como el framework propuesto.

Mejores prácticas de DevOps para aplicaciones escalables: Estudios como el de Smith (2022) han demostrado cómo la integración de Docker y Kubernetes en entornos de desarrollo mejora la capacidad de adaptación y la escalabilidad en organizaciones privadas. Docker es ampliamente considerado un marco estándar para la reubicación de aplicaciones, lo cual sugiere que cualquier desarrollo orientado a facilitar la migración entre entornos debería considerar el uso de tecnologías de contenerización. Esto es fundamental para la estrategia de migración de ambientes de producción en entidades públicas.

Adopción de DevOps en Pequeñas y Medianas Empresas (PyMEs): Un proceso validado para adoptar DevOps en PyMEs aborda la falta de estandarización y la diversidad en prácticas, definiendo actividades, roles y herramientas para automatizar la integración y monitoreo continuo. Aunque enfocado en PyMEs, los hallazgos de Certuche, Zúñiga, Pardo, & Orozco (2022) son extrapolables a entidades públicas que enfrentan desafíos similares, como restricciones presupuestarias y dependencia de personal técnico especializado, siendo relevantes para la estandarización y optimización de la migración.

Aplicación de IA en la administración pública: Proyectos como el desarrollado por el Gobierno de Estonia, referenciado por Jones et al. (2021), han integrado sistemas inteligentes para automatizar servicios públicos, garantizando mayor precisión y reducción de tiempos. Esto valida la aplicabilidad de la IA en el sector público para mejorar procesos operativos complejos, incluyendo la gestión de la migración de sistemas.

Optimizando la gestión de modelos de IA en entornos en la nube: Desafíos y soluciones. Este artículo de Nuguri et al. (2021) analiza los retos y soluciones asociados a la gestión y reubicación de modelos de inteligencia artificial en entornos de nube. Identifica problemas clave como la gestión de recursos computacionales, la privacidad de datos, la interoperabilidad entre proveedores de nube, y el rendimiento de los modelos. Propone estrategias como la compresión y poda de modelos, el aprendizaje federado, y el uso de contenedores para garantizar escalabilidad y eficiencia. El estudio enfatiza la importancia de las arquitecturas nativas en la nube para reducir costos y destaca el uso de estándares abiertos para facilitar la migración entre proveedores. También resalta la necesidad de una monitorización y actualización continua para mantener la efectividad en entornos dinámicos, aspectos directamente aplicables al framework de migración con IA.







Bases Teóricas

La presente investigación se fundamenta en conceptos esenciales vinculados a la Inteligencia Artificial (IA), la automatización de procesos de software y la gestión de infraestructuras para la migración de sistemas. Estos pilares conceptuales son cruciales para comprender la propuesta de un framework diseñado para optimizar la transición de aplicaciones web en entornos críticos como el sector público.

Transformación Digital

La Transformación Digital se describe como un proceso de adaptación a las nuevas tecnologías con el fin de mejorar los modelos de negocio (Vial, 2019). En el ámbito del sector público, esta transformación busca optimizar los procesos internos para incrementar la eficiencia y reducir costos. La migración de sistemas representa un pilar fundamental en este cambio, ya que permite a las entidades modernizar su infraestructura tecnológica y, consecuentemente, los servicios digitales que ofrecen. Su relevancia en este estudio radica en que contextualiza la urgencia y el mandato que impulsan la necesidad de optimizar la migración de aplicaciones en entidades como PROMPERÚ.


Agnosticismo del Proveedor y Reubicación de Sistemas de Información
Según el estándar ISO/IEC 25010 (2011), la capacidad de reubicación de un sistema se refiere a su aptitud para ser transferido de un entorno a otro sin requerir modificaciones significativas. En el sector público, esta característica es indispensable debido a la necesidad de migrar sistemas entre diversos proveedores de servicios de alojamiento o plataformas en la nube, promoviendo así la independencia tecnológica. Esto se materializa en el concepto de agnosticismo del proveedor, fundamental para evitar dependencias tecnológicas y asegurar la flexibilidad operativa.

Herramientas clave para la Reubicación de Sistemas:

Infraestructura como Código (IaC): Esta práctica permite la gestión y el aprovisionamiento de la infraestructura mediante código, lo cual facilita la reproducibilidad y la reubicación de entornos. IaC es fundamental para automatizar la preparación del ambiente de destino en un proceso de migración.
Arquitectura de Microservicios: Este enfoque consiste en construir aplicaciones como un conjunto de servicios pequeños e independientes. Esto incrementa la modularidad y facilita la migración de componentes individuales o el cambio de entornos de forma incremental, reduciendo la complejidad del proceso.


 Automatización de Migraciones de Software
La automatización de migraciones emplea herramientas y scripts para trasladar aplicaciones y sus datos a nuevos entornos de producción sin intervención manual (Humble & Farley, 2010). Este proceso asegura la consistencia, reduce los tiempos de transferencia y minimiza los errores, elementos críticos para la continuidad operativa de las aplicaciones en el sector público.

Herramientas clave para la Automatización de Migraciones:
Pipeline de Integración Continua / Entrega Continua (CI/CD): Este modelo automatiza el flujo de trabajo desde la integración del código hasta su preparación para el ambiente de destino. Incluye pasos automatizados de pruebas, compilación y transición de sistemas, asegurando un proceso de migración fluido.
Contenerización: El uso de herramientas como Docker para encapsular aplicaciones junto con todas sus dependencias en unidades aisladas y transportables (contenedores). Estos contenedores pueden ejecutarse consistentemente en cualquier entorno que los soporte, simplificando significativamente el proceso de migración y mitigando problemas de compatibilidad.

Gestión de Recursos y Escalabilidad
Los entornos de nube emplean estrategias de escalabilidad horizontal y vertical para ajustar dinámicamente los recursos según las necesidades del sistema. Este concepto es esencial en sistemas inteligentes para garantizar el rendimiento y la eficiencia de las aplicaciones tras una migración y durante su operación continua.

Herramientas clave:
Orquestadores de Contenedores: Herramientas como Kubernetes automatizan la gestión de aplicaciones distribuidas, incluyendo su escalado y asignación dinámica de recursos. Son fundamentales para la gestión de ambientes post-migración y para asegurar que las aplicaciones funcionen con la capacidad y disponibilidad adecuadas.
Bases de Datos Distribuidas: Tecnologías como Redis permiten manejar grandes volúmenes de datos y consultas de manera eficiente, lo cual es vital para soportar la infraestructura de aplicaciones migradas que demandan alta disponibilidad y rendimiento.

Inteligencia Artificial (IA) en la Administración Pública
La Inteligencia Artificial (IA) se define como la rama de la informática que desarrolla algoritmos y sistemas capaces de realizar tareas que tradicionalmente requerían inteligencia humana, como el aprendizaje, la resolución de problemas y la toma de decisiones. En el sector público, la IA ha demostrado su utilidad para mejorar procesos administrativos y servicios al ciudadano. Estudios como los de Nuguri et al. (2021) destacan su impacto en la automatización, la optimización de recursos y la reducción de errores en entornos críticos. La aplicación de la IA en la gestión de la migración de aplicaciones representa una oportunidad para transformar un proceso complejo y propenso a fallos en una operación eficiente, adaptable y controlada.

Herramientas clave de IA para la Migración:
Machine Learning (Aprendizaje Automático): Son algoritmos que permiten a los sistemas aprender patrones a partir de datos históricos. En el contexto de la migración, pueden optimizar la toma de decisiones, generar planes de migración y detectar anomalías basándose en experiencias previas o configuraciones de ambientes.
Reinforcement Learning (Aprendizaje por Refuerzo): Estas estrategias de aprendizaje, basadas en recompensas, optimizan la toma de decisiones en entornos complejos y dinámicos. Potencialmente aplicables para afinar rutas de migración o manejar eventos inesperados durante el proceso, contribuyendo a una migración más resiliente.




Bases Conceptuales

Las siguientes definiciones conceptuales establecen el vocabulario clave y los marcos teóricos específicos que fundamentan la presente investigación sobre la optimización de la gestión de la migración de aplicaciones web mediante un framework basado en inteligencia artificial.

Inteligencia Artificial (IA): Según Russell & Norvig (2020), la inteligencia artificial se entiende como la capacidad de un sistema de cómputo para ejecutar operaciones que tradicionalmente requieren de la inteligencia humana, tales como el aprendizaje, el análisis de datos y la resolución de problemas. En esta tesis, se refiere a la aplicación de algoritmos y técnicas que permiten al framework aprender y optimizar los procesos de migración.

DevOps: Proveniente de la combinación de "Dev" (desarrollo) y "Ops" (operaciones), DevOps es un paradigma que implementa la integración continua con el objetivo de automatizar la transición de software en ambientes ya establecidos (Banala, S., 2024). Para este estudio, es fundamental por su énfasis en la automatización, colaboración y mejora continua aplicadas a los procesos de migración.

Transformación Digital: La transformación digital es el proceso de integrar tecnologías digitales en todas las áreas de una organización para cambiar fundamentalmente cómo opera y el valor que ofrece a sus usuarios (Vial, 2019). En el contexto de las entidades públicas, esta transformación impulsa la necesidad de modernizar y optimizar la migración de sistemas para mejorar la eficiencia y los servicios al ciudadano.

Automatización de Procesos: Consiste en el uso de tecnología para realizar tareas de manera automática, lo que contribuye a la reducción de errores y la optimización de tiempos (Hernández Yeja & Porven Rubier, 2016). Aplicado a esta investigación, se refiere a la capacidad del framework para ejecutar tareas de migración de forma autónoma y consistente.

Reubicación de Sistemas: Se define como la capacidad de un sistema para ser trasladado entre diferentes entornos sin experimentar una pérdida significativa de funcionalidad o rendimiento (Abied et al., 2022). Este concepto es crucial para la migración de aplicaciones web entre proveedores o infraestructuras, asegurando la continuidad operativa y la independencia tecnológica.

Gestión de Migraciones de Software: Se refiere al proceso sistemático de mover aplicaciones y sus componentes de un entorno operativo a otro, asegurando su funcionalidad, integridad y compatibilidad en el nuevo ambiente (Kolltveit & Li, 2022, adaptado). En el marco de esta tesis, implica la planificación, ejecución y control de todas las actividades necesarias para una transición exitosa de aplicaciones web.



HIPÓTESIS Y VARIABLES

Hipótesis general

El desarrollo e implementación de un framework basado en inteligencia artificial optimizará la gestión de la migración de aplicaciones web en entidades públicas peruanas, específicamente en PROMPERÚ, lo que resultará en la garantía de la continuidad operativa, la reducción significativa de los tiempos de transferencia y la minimización de errores durante el proceso de migración.

Hipótesis especificas

Estas hipótesis detallan las suposiciones específicas que la investigación busca validar respecto al desarrollo y el impacto del framework de migración impulsado por IA:

La identificación exhaustiva de los requisitos funcionales y no funcionales, así como de los puntos críticos y dependencias en los ambientes de producción de PROMPERÚ, es indispensable para el diseño efectivo de un framework de gestión de migración de aplicaciones web.

Esta hipótesis postula que un análisis inicial minucioso es un requisito previo para un diseño exitoso del framework.

El diseño de una arquitectura y componentes de un framework de gestión de migración que incorpore inteligencia artificial permitirá la generación automatizada de planes de migración optimizados, reduciendo significativamente la dependencia del conocimiento individual del personal técnico.

Esta hipótesis afirma que el diseño impulsado por IA conducirá a planes de migración automatizados y mejorados, disminuyendo así la dependencia de la experiencia humana específica.

La implementación exitosa de los módulos clave del framework propuesto facilitará la aplicación automatizada de los planes de migración y asegurará una trazabilidad completa de todas las actividades, mejorando sustancialmente el control y la transparencia del proceso.

Esta hipótesis establece que el framework implementado automatizará la ejecución de los planes y proporcionará una trazabilidad completa, lo que resultará en un control mejorado.

La evaluación del framework propuesto en un entorno relevante (simulado o piloto en PROMPERÚ) demostrará su efectividad en la optimización de la continuidad operativa, la reducción de los tiempos de transferencia y la minimización de errores durante los procesos de migración de aplicaciones web.

Esta hipótesis sostiene que la fase de prueba demostrará empíricamente la capacidad del framework para lograr las mejoras deseadas en el rendimiento de la migración.







Identificación de variables

Variable Independiente: 

Framework de Gestión de Migración de Aplicaciones Web Basado en Inteligencia Artificial.

Definición: Esta es la "solución" o la "intervención" que tu tesis está desarrollando y proponiendo. Es el elemento que tú manipulas (a través de su diseño e implementación) para observar un efecto. Incluye las características clave del framework: análisis de estado, generación de planes, aplicación de planes, trazabilidad y el uso de IA.

Variable Dependiente:

Optimización de la Gestión de la Migración de Aplicaciones Web.

Definición: Esta es la variable que se espera que cambie o mejore como resultado de la aplicación del framework. 

La "optimización" se manifestará en indicadores específicos que son tus dimensiones de medida:

Continuidad Operativa: La capacidad de los sistemas de PROMPERÚ de permanecer disponibles y funcionales durante y después del proceso de migración.

Reducción de Tiempos de Transferencia: La disminución del tiempo necesario para completar el proceso de migración de las aplicaciones web.

Minimización de Errores: La disminución en la cantidad o frecuencia de fallos técnicos, inconsistencias o problemas que ocurren durante las migraciones.



Operacionalización de variables








Matriz de consistencia


Referencias Bibliográficas:


Niño-Martínez, V. M., Ocharán-Hernández, J. O., Limón, X., & Pérez-Arriaga, J. C. (2022). A microservice deployment guide. Universidad Veracruzana, School of Statistics and Informatics.

Abied, X., et al. (2022). Building a framework to drive government systems’ adoption of cloud computing through IT knowledge. Sustainability, 14, 15590.

Hernández Yeja, A., & Porven Rubier, J. (2016). Procedimiento para la seguridad del proceso de despliegue de aplicaciones web. Revista Cubana de Ciencias Informáticas, 10(2), 42-56

Romero-Álvarez, J., Alvarado-Valiente, J., Moguel, E., Garcia-Alonso, J., & Murillo, J. M. (2024). Enabling continuous deployment techniques for quantum services. Software: Practice and Experience, 54(8), 1491-1515

Haidar, A. (2024). An Integrative Theoretical Framework for Responsible Artificial Intelligence. International Journal of Digital Strategy, Governance, and Business Transformation, 13(1), 1–18

Korontanis, I., Makris, A., & Tserpes, K. (2024). A Survey on Modeling Languages for Applications Hosted on Cloud-Edge Computing Environments. Applied Sciences, 14(6), 2311

Russell, S., & Norvig, P. (2020). Artificial Intelligence: A Modern Approach (4ª ed.). Pearson.

Jones, R., Smith, L., & Brown, T. (2021). Artificial Intelligence in Public Administration: A Case Study of Estonia's E-Government System. Journal of Digital Governance, 12(3), 45-62. DOI: 10.1016/j.jdigov.2021.03.004.

Smith, A. (2022). DevOps Best Practices for Scalable Applications. Software Architecture and Design Journal, 10(1), 32-47.

Banala, S. (2024). DevOps Essentials: Key Practices for Continuous Integration and Continuous Delivery. Double Blind Peer Reviewed Journal, Impact Factor: 7.8.

Certuche, S. C., Zúñiga, K., Pardo, C., & Orozco, C. (2022). Proceso para fomentar y apoyar la adopción de DevOps en PyMEs de software. Revista Científica, 45(3), 422-437

Nuguri, S., Saoji, R., Shiva, K., Etikani, P., & Bhaskar, V. V. S. R. (2021). Optimizing AI Model Deployment in Cloud Environments: Challenges and Solutions. International Journal for Research Publication & Seminar, 12(2), 159-167

Tudela Aranda, J. (2023). Gobierno, parlamento, democracia e inteligencia artificial. Teoría y Realidad Constitucional, (52), 303-333.


Humble, J., & Farley, D. (2010). Continuous Delivery: Reliable Software Releases through Build, Test, and Deployment Automation. Addison-Wesley.

ISO/IEC. (2011). ISO/IEC 25010:2011 Systems and Software Engineering – Systems and Software Quality Requirements and Evaluation (SQuaRE) – System and Software Quality Models.

Kim, G., Humble, J., Debois, P., & Willis, J. (2016). The DevOps Handbook. IT Revolution Press.

Russell, S., & Norvig, P. (2020). Artificial Intelligence: A Modern Approach (4ª ed.). Pearson.

Nuguri, S., Saoji, R., Shiva, K., Etikani, P., & Bhaskar, V. V. S. R. (2021). Optimizing AI Model Deployment in Cloud Environments: Challenges and Solutions. International Journal for Research Publication & Seminar, 12(2), 159-167.

Kolltveit, A. B., & Li, J. (2022). Operationalizing Machine Learning Models - A Systematic Literature Review. Workshop on Software Engineering for Responsible AI (SE4RAI’22), Pittsburgh, PA, USA. ACM. 

Akbar, M. A., Khan, A. A., Islam, N., & Mahmood, S. (2023). DevOps project management success factors: A decision-making framework. Software: Practice and Experience, 54(2), 257–280. 

Vial, G. (2019). Understanding digital transformation: A review and a research agenda. The Journal of Strategic Information Systems, 28(2), 118-144




Anexos:










