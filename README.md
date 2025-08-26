# Trabajo Práctico Final  
**Usabilidad y Diseño Centrado en el Usuario para Sistemas de IA**
**Estudiante:** Rodrigo Otárola Gutiérrez 
**Sistema elegido:** Claude AI

---

## Fase 1: Análisis inicial

### Descripción del sistema
Claude AI es es un modelo de lenguaje natural(LLM) de última generación diseñado para comprender y generar texto con un alto grado de precisión y fluidez. Este modelo se ha desarrollado para abordar las limitaciones observadas en versiones anteriores de modelos LLM, ofreciendo mejoras significativas en términos de velocidad, rentabilidad, inteligencia contextual y capacidad para manejar grandes volúmenes de datos.

### Usuarios principales
- **Usuario 1: Profesionales e investigadores**  
  Utiliza este LLM para tareas de redacción, análisis, investigación y síntesis de información  
  **Necesidades:** Respuestas confiables con mayor contexto y explicación del razonamiento.  
  **Limitaciones:** Conocimiento con corte a Enero 2025 y riesgo de sobreconfianza.
- **Usuario 2: Estudiantes y educadoras**  
  Utiliza este LLM para Programación, explicaciones educativas, asistencia académica.  
  **Necesidades:** Precisión técnica con explicaciones comprensibles.  
  **Limitaciones:** Puede inhibir el desarrollo del pensamiento crítico independiente y no conoce planes academicos.
- **Usuario 3: Usuarios generales/técnicos**  
  Utiliza este LLM para programación, documentación, resolución de problemas técnicos.  
  **Necesidades:** Código más limpio, bien documentado y documentación técnica.  
  **Limitaciones:** Pruede desconocer versiones modernas de algunos framework, no tiene entorno de ejecución de pruebas.

### Riesgos éticos y de sesgo
- **Alucinaciones:** Genera información que suena creíble pero puede ser incorrecta, especialmente en temas técnicos específicos.  
- **Sobreconfianza:** Usuarios pueden asumir que las respuestas articuladas de Claude son siempre precisas, sin verificación independiente.  
- **Sesgo cultural occidental:** Predominio de perspectivas occidentales en respuestas, con menor representación de culturas no occidentales.  
- **Privacidad de datos:** Riesgo al compartir información personal o sensible en las consultas, que se procesan en servidores externos.

---

## Fase 2: Evaluación de usabilidad

### Aplicación de heurísticas (Nielsen adaptadas a IA)
- **Visibilidad del estado:** Al esperar respuesta solo se visualiza un icono de similar a cargando, llega a mostrar fuentes de información con sus links.  
- **Correspondencia con el mundo real:** Es lenguaje natural, similar al humano, pero en momentos es muy extenso y técnico, dependera del contexto de la pregunta.  
- **Control y libertad del usuario:** Posee opción de detener la respuesta y de editar las preguntas.  
- **Consistencia y estándares:** Interfas e iconografía clara.  
- **Prevención de errores:** Puede solicitas imagen en caso de señalarla en la pregunta, pero noo advierte de manera clara cuando la información puede ser no confiable.  
- **Reconocer mejor que recordar:** Permite ocultar las conversaciones anteriores y mantiene visualizador de respuestas para usuarios técnicos como programadores bastante legible.  
- **Flexibilidad y eficiencia:** Usuarios avanzados busquedas más complejas, pero usuarios normales puede obtener buenos resultados con técnicas no tan avanzadas.  
- **Estética y minimalismo:** Intefaz buena, respuestas puedes ser extensas y en algunos casos visualizar un editar lateral.  
- **Ayuda y documentación:** Posee FAQ (preguntas frecuentes) o "trucos" para usuarios iniciales.  
- **Reconocer, diagnosticar y recuperarse de errores:** En caso de errores de red o exceder los tokens de usuario gratuito, el usuario debe crear nuevo chat.

### Problemas de usabilidad detectados
1. **Falta de relación de información entre chats:** No se puede interrelacionar preguntas de otros chats del mismo usuario, cada chats es independiente.  
2. **Ausencia de historial de búsqueda:** No permite buscar dentro del historial de conversaciones previas para encontrar información específica ya discutida. 
3. **Falta de control sobre respuestas:**  No hay opciones para especificar longitud deseada, nivel de detalle, o formato antes de generar la respuesta, obligando a regenerar múltiples veces.

---

## Fase 3: Propuesta de mejora

### Problema 1 → Falta de relación de información entre chats
- **Mejora:** Etiquetado y vinculación que permita conectar conversaciones relacionadas con referencias cruzadas automáticas.  
- **Beneficio:** Construcción de conocimiento personalizado.

### Problema 2 → Ausencia de historial de búsqueda
- **Mejora:** Función de búsqueda global en historial con distintos filtros(fechas, temas u otros).  
- **Beneficio:** Recuperación de infomación y gestión de conocimiento de cada usuario.

### Problema 3 → Falta de control sobre respuestas
- **Mejora:** Panel de configuración pre-respuesta con controles para longitud, tecnicismo y formato.  
- **Beneficio:** Respuestas personalizadas que se adaptan al contexto y nivel de expertise del usuario.

---

## Fase 4: Plan de validación

### Método principal 
- **Evaluación heurística adaptada:** Revisión exhaustiva con los usuarios del sistema.  
- **Pruebas con usuarios (mínimo 10):**  
  - 7 novatos
  - 3 avanzados

### Tareas de prueba
1. Buscar información de una conversación anterior usando el historial de búsqueda.  
2. Crear una pregunta compleja y ajustar configuraciones de respuesta (longitud/tecnicismo) antes de enviar.
3. Vincular información de dos chats diferentes usando el sistema de etiquetado.
4. Regenerar una respuesta cambiando solo el nivel de detalle sin reescribir la pregunta.
Identificar y seguir una referencia cruzada automática hacia un chat relacionado.

---

## Conclusiones

El análisis realizados a Claude AI, si bien posea una interfaz clara y respuestas efectivas, presenta limitaciones en gestión de información personalizada y maás problemas que impactan en la experiencia de usuario con distintos niveles de seniority, generando ineficiencias y potencial sobreconfianza. Las mejoras propuestas son técnicamente viables y abordan necesidades reales, con un plan de validación apropiado que permitiría implementar funcionalidades de gestión de conocimiento sin alterar el modelo base.

---
