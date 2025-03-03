#####################################################################################
#####################################################################################
#                                                                                   #
#                 Bienvenido/a a la calculadora de hipotecas inversas               #
#                                                                                   #
#   Fecha: 16/01/2025                                                               #
#   Versión: 1.0                                                                    #
#                                                                                   #
#   El código de este programa está pensado para cargar el entorno y las bases      #
#   de datos directamente desde el script. Si por alguna razón el código diese      #
#   problemas en lo relativo al entorno, puedes cargarlo manualmente desde los      #
#   archivos adjuntos en la carpeta.                                                #
#                                                                                   #
#   Dataframe:  VIVIENDA.xlsx   TABLA_VIDA.xlsx                                     #
#   Funciones:  Funciones_entorno.txt                                               #
#   Values:     Los valores se introducen mediante el programa                      #
#                                                                                   #
#   El programa requiere algo de CPU y potencia computacional, si en algún          #
#   paso parece que se queda colgado, revisa en el administrador de tareas          #
#   si R Studio está consumiendo CPU, o el consumo es superior al 5-6%,             #
#   significa que el programa está calculando; en caso contrario, es que algo en    #
#   el código ha fallado.                                                           #
#                                                                                   #
#   El trabajo ha consistido en una parte teórica y una parte práctica. La          #
#   parte teórica consiste en el desarrollo del modelo matemático-actuarial         #
#   que he utilizado para realizar el programa. NO ES ESTRICTAMENTE NECESARIO       #
#   LEER LA PARTE TEÓRICA DEL TRABAJO. La parte práctica, por otro lado,            #
#   consiste en modificar bases de datos del INE y procesar datos necesarios        #
#   para nutrir el programa. Luego, implementar las funciones del modelo,           #
#   "lo cual ha sido una hazaña remarcable". Entre ellas, he tenido que aprender    #
#   algo de métodos numéricos. En particular, el único método numérico que ha       #
#   resultado útil ha sido el algoritmo Newton-Raphson multidimensional.            #
#   Finalmente, he creado el código principal, un programa interactivo que carga    #
#   los pasos anteriores en el entorno de R y ofrece resultados.                    #
#                                                                                   #
#   El código principal funciona de la siguiente manera:                            #
#   1. Toma de datos.                                                               #
#   2. Procesa los datos utilizando dataframes y funciones.                         #
#   3. Selecciona uno de los dos métodos de análisis.                               #
#   4. Realiza el análisis mediante métodos numéricos, tablas y plots.              #
#   5. Te permite volver al inicio del programa para volver a calcular.             #
#                                                                                   #
#   Este trabajo ha requerido prácticamente la totalidad de mi tiempo desde         #
#   navidades. He de decir que estoy relativamente satisfecho con el resultado,     #
#   aunque creo que aún podrían mejorarse muchas cosas. Sin duda, la parte más      #
#   compleja del trabajo ha sido desarrollar el modelo desde 0 y tratar de          #
#   interpretarlo. El modelo acaba llegando a una conclusión que se resume          #
#   en un modelo de ecuaciones no lineales y no analíticas que no tienen solución   #
#   mediante los métodos de cálculo habituales. Por eso ha sido necesario           #
#   investigar métodos numéricos para poder calcular las primas de riesgo.          #
#                                                                                   #
#   Además, diseñar y poner en práctica todas las funciones ha sido una tarea       #
#   compleja. En particular, vector_val_H() ha sido bastante complejo de programar  #
#   debido a la cantidad de excepciones que tiene. newtonraphson_rktcontr(),        #
#   por otro lado, ha sido complicado debido a que he tenido que aprender desde 0   #
#   cómo funciona el algoritmo. Aunque es un algoritmo famoso y había muchas        #
#   fuentes, su implementación no fue sencilla.                                     #
#                                                                                   #
#   El código puede parecer algo incomprensible a primera vista, no lo niego. Por   #
#   eso es importante ejecutarlo desde source para simplemente dirigirlo desde la   #
#   consola de R Studio. En principio, todo debería acabar dando resultados.        #
#                                                                                   #
#   Finalmente, la memoria no está todo lo bien que me gustaría, pero es todo lo    #
#   que me ha dado tiempo a hacer desde el día 22 de diciembre. Es posible que la   #
#   modifique como parte de una publicación más extensa.                            #
#                                                                                   #
#                                                                                   #
#   Gracias por la atención!                                                        #
#                                                                                   #
#                                                                                   #
#   Sergi López Vergara                                                             #
#                                                                                   #
#####################################################################################
#####################################################################################
#####################################################################################

