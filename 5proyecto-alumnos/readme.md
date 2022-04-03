# Proyecto de alumnos matriculados.

Elaborado por: Alejandro Acosta León  
Email: alejo.a1990@gmail.com

---

Este proyecto busca predecir la probabilidad de matriculación de alumnos de pregrado de una universidad privada del Ecuador en función de algunas características de los estudiantes.  

La variable dependiente (**doc**) representa el estado del candidato. Toma el valor de 1 para estudiantes que se enrolaron en la universidad y 0 caso contrario.  

La base de datos ha sido anonimizada, tanto nombres, identificaciones de candidatos y funcionarios fueron eliminados o codificada (utilizando funciones hash). Esto mantiene la privacidad de al información.  

Para obtener los datos, se utilizó SimpleSalesforce, librería de python que permite extraer datos directamente del CRM que maneja la institución educativa. Este proceso se lo hizo previamente por motivos de privacidad, aquí se utiliza un archivo más limpio y trabajado.

Una vez que procesados los datos, las variables explicativas son las siguientes:
 - **id_oportunidad** : identificador de la oportunidad, oportunidad es la combinación entre candidato e interés
 - **id_estudiante** : identificador del estudiante
 - **programa** : código del programa académico
 - **etapa** : estado actual del postulante (afluente, inscrito, test, matriculado, perdido)
 - **fecha_afluencia** : fecha de primera consultoría
 - **fecha_cierre** : fecha de finalización del proceso de admisión (se gana o se cierra)
 - **ciclo** : tiempo en días transcurrido entre la fecha de afluencia y la de cierre
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