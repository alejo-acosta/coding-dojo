# Proyecto de alumnos matriculados.

Elaborado por: Alejandro Acosta León  
Email: alejo.a1990@gmail.com

---

Este proyecot busca predecir la probabilidad de matriculación de alumnos de pregrado de una universidad privada del Ecuador en función de algunas características de los estudiantes.  

La variable dependiente (**doc**) representa el estado del candidato. Toma el valor de 1 para estudiantes matriculados y 0 caso contrario.  

La base de datos ha sido anonimizada, tanto nombres e identificaciones de candidatos como de funcionarios fueron eliminados o codificada (utilizando funciones hash). Esto mantiene la privacidad de al infomación.  

Para obtener los datos, se utilizó una librería de python que permite extraer datos directamente del CRM de la institución educativa. Este proceso se lo hizo previamente por motivos de privacidad, se trabaja con un archivo más trabajado.

Una vez que se procesan los datos, las variables explicativas se describen a continuación:
 - **id_oportunidad** : identificador de la oportunidad
 - **id_estudiante** : identificador del estudiante
 - **programa** : código del programa académico
 - **etapa** : estado actual del postulante (afluente, inscrito, test, matriculado, perdido)
 - **fecha_afluencia** : fecha de primera consultoría
 - **fecha_cierre** : fecha de finalización del proceso de admisión (se gana o se cierra)
 - **ciclo** : tiempo transcurrido entre la fecha de afluencia y la de cierre
 - **consultor** : código del consultor que le atendió
 - **edad** : edad del postulante
 - **estado_civil** : estado civil del postulante
 - **ciudad** : ciudad de residencia
 - **provincia** : provincia de residencia
 - **trabaja** : 1 si trabaja, 0 caso contrario
 - **colegio** : código del colegio donde estudió
 - **tipo_admision** : tipo de admisión
    - Normal, Convalidado, Intercambio, Especial
 - **origen** : de donde se obtuvo la información del postulante (redes sociales, colegios, llamada, etc.)
 - **enteraste** : ¿cómo te enteraste de la universidad?