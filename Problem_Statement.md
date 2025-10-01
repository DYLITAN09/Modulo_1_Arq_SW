**Problem Statement con objetivos, métricas y riesgos.**

**Declaración del Problema** <br>
El principal reto que enfrentan las administraciones tributarias y aduaneras (ATyA) es la evasión fiscal en el comercio exterior. Esta se da a través de prácticas como declarar valores más bajos de los reales, realizar exportaciones falsas o alterar el origen de las mercancías. Todo esto reduce la recaudación y genera competencia desleal, ya que algunas empresas obtienen ventajas indebidas al evadir impuestos, mientras que otras cumplen con todas sus obligaciones fiscales.
Este problema se ve agravado por:

1. La falta de integración entre los controles aduaneros y fiscales, lo que dificulta la detección de fraudes. 

2. La fragmentación de los sistemas de control, incluso dentro de una misma entidad, que conduce a la duplicación de esfuerzos y errores.

3. La carencia de cooperación efectiva entre las ATyA, que impacta negativamente la trazabilidad de las cadenas de suministro a nivel local y global.

La F-eCX es la transformación digital propuesta para integrar los datos de exportaciones e importaciones, buscando mejorar la recaudación y el control del IVA en transacciones internacionales.

**Objetivos (Goals)** <br>
El objetivo principal de este proyecto, financiado mediante un Bien Público Regional (BPR) RG-T4185 del BID, es desarrollar e implementar un piloto (fase de prueba) de una solución digital para la emisión y gestión de la F-eCX, apalancándose en el uso de credenciales verificables.

**Objetivos Estratégicos y de Solución:** <br>
**1. Mejorar la Recaudación y el Control:** Fortalecer los mecanismos de gestión de riesgos, verificación e inspección, poniendo a disposición de las ATyA información valiosa y verificable de manera oportuna.<br>

**2. Integración Nacional e Internacional:** <br>
- Integrar los controles de la administración tributaria y aduanera en el país de exportación.<br>
- Interconectar los controles aduaneros entre los países de exportación e importación.<br>
- Integrar los controles aduaneros y fiscales en el país de importación.<br>

**3. Facilitación del Comercio:** Simplificar el proceso regulatorio y facilitar la conversión de datos, lo que fomenta el ahorro de tiempo y recursos financieros para el sector privado.<br>

**4. Armonización Tecnológica:** Diseñar e implementar una solución tecnológica que utilice Credenciales Verificables (VCs) e Identificadores Descentralizados (DIDs), siguiendo los estándares de la W3C, y que sea adaptable a las necesidades de los países participantes.

**Métricas y Resultados (Metrics and Expected Outcomes)** <br>
Aunque las fuentes no detallan las métricas cuantitativas específicas de rendimiento (KPIs), el proyecto define los siguientes indicadores de resultados y áreas de evaluación para validar el éxito del piloto:

<img width="763" height="561" alt="image" src="https://github.com/user-attachments/assets/ee00bba3-8616-4906-93d8-04384b543aa5" />


**Riesgos y Restricciones (Risks and Constraints)** <br>
Los riesgos y limitaciones del proyecto están intrínsecamente ligados a su alcance como piloto y a sus requisitos tecnológicos obligatorios:

**Riesgos Operacionales y de Alcance (Limitaciones del Piloto):** <br>
**1. Limitación del Piloto:** El alcance es la implementación de un piloto en un entorno de prueba (ambiente de calidad), utilizando datos ficticios que simulan operaciones reales, sin efectos jurídicos. Esto conlleva el riesgo inherente de la transición a un ámbito real de operación.<br>

**2. Participación Limitada:** El piloto debe contemplar la participación de las ATyA de 2 o 3 países y de 2 o 3 empresas seleccionadas.<br>

**3. Dependencia de la F-eX:** El modelo presupone la existencia de la emisión de la F-eX en una fase previa al despacho de exportación. La falta de una F-eX reduce los beneficios de la integración entre las administraciones tributarias y aduaneras.<br>

**4. Armonización Legal/Regulatoria:** Existe el riesgo de que el marco normativo doméstico e internacional actual no contemple todas las facultades necesarias para ejecutar las operaciones definidas, requiriendo un análisis exhaustivo y posibles cambios normativos.<br>

**5. Exclusiones del Piloto (Simplificación):** Para simplificar el piloto, se recomienda eliminar o simplificar ciertas funcionalidades complejas:<br>

- La rectificación de la F-eCX (antes de su vinculación a una D-eX) se realizará mediante la cancelación y emisión de una nueva F-eCX.<br>
- Se elimina el tratamiento de las rectificaciones de la F-eCXe después de la finalización del despacho de exportación.<br>
- Se elimina el tratamiento de las divergencias entre el exportador y el importador (Sección 13).<br>

**Riesgos Tecnológicos y de Estándares:** <br>
**1. Tecnología Mandatoria:** El sistema debe usar Credenciales Verificables (VCs) e Identificadores Descentralizados (DIDs), siguiendo los estándares de la W3C, lo cual es una tecnología relativamente nueva en este contexto.

**2. Código Abierto:** Todos los componentes de la solución deben estar basados en código abierto, según los requerimientos del BID.

**3. Fallo de Integridad de Datos:** El sistema fallará si no puede asegurar la autenticidad y validez de los archivos digitales, o la integridad de la información desde la emisión de la F-eX hasta la F-eCXm. La F-eCX debe permitir la verificación descentralizada de su integridad.

**4. Modelo de Datos Incompleto:** El Modelo de Datos de la Organización Mundial de Aduanas (OMA), si bien es una referencia obligatoria, puede ser insuficiente para los intereses del control fiscal interno, lo que requiere que se mantengan datos de interés nacional.

**5. Costo Estimado:** El proyecto cuenta con un Presupuesto estimado de US$ 150,000.00.
