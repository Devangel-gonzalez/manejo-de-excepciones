**Angel Israel Gonzalez Torres**

Ejecutar primero con un archivo válido y después con un archivo que contenga:

85  
90  
abc  
75

# Registrar

**1. ¿Qué excepción aparece?**

85  
90  

    Exception in thread "main" java.lang.NumberFormatException: For input string: "abc"
        at java.base/java.lang.NumberFormatException.forInputString(NumberFormatException.java:67)
        at java.base/java.lang.Integer.parseInt(Integer.java:662)
        at java.base/java.lang.Integer.parseInt(Integer.java:778)
        at ProcesadorCalificaciones.main(ProcesadorCalificaciones.java:17)

Cuando se ejecuta un documento con los datos
85
90
abc
75

**2. ¿En qué línea ocurre?**
En la linea 17 como muestra el error
        
    at ProcesadorCalificaciones.main(ProcesadorCalificaciones.java:17)

en el codigo    
    
    int calificacion = Integer.parseInt(linea);  

**3. ¿Continúa la ejecución?**

No porque la excepción no esta manejada y si siguiera ejecutándose, hubiera impreso 75

**4. ¿Qué información proporciona el stack trace?**

- Falló porque intentó convertir una cadena de texto "abc" en un número

      java.lang.NumberFormatException: For input string: "abc"

- Te dice el nombre del archivo y la linea donde fallaron:  **ProcesadorCalificaciones** y **17**
  
      at ProcesadorCalificaciones.main(ProcesadorCalificaciones.java:17)






