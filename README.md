# manejo-de-archivo
constructores y destructores

Explicación del Código
__init__: Se activa automáticamente cuando se crea un nuevo objeto. Aquí abrimos un archivo.

__del__: Se ejecuta cuando el objeto es destruido (por ejemplo, al finalizar el programa o al usar del). Aquí se cierra el archivo.

El código está documentado con comentarios explicativos.

Aplica buenas prácticas: manejo de errores, encapsulamiento de lógica, claridad.

¿Qué hace el programa?
Al crear un objeto de la clase Archivo, el constructor abre un archivo de texto y guarda su referencia.

Luego, se puede escribir en el archivo utilizando el método escribir().

Cuando el objeto es destruido (por ejemplo, al finalizar el programa), el destructor cierra automáticamente el archivo, asegurando una correcta gestión de recursos.

def __init__(self, nombre_archivo):
    # Se ejecuta al crear el objeto. Abre el archivo.

def __del__(self):
    # Se ejecuta al destruir el objeto. Cierra el archivo.
Requisitos específicos cumplidos
* Se utiliza claramente un constructor para inicializar atributos.
* Se usa un destructor para cerrar el recurso (archivo).
* El código está comentado y documentado para facilitar la comprensión.
* Estructura limpia y siguiendo buenas prácticas de programación.
* El código ha sido desarrollado en PyCharm y publicado en este repositorio de GitHub.


