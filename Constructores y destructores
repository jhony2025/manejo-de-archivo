class Archivo:
    """
    Clase que representa el manejo de un archivo de texto.
    Utiliza un constructor para abrir el archivo y un destructor para cerrarlo.
    """

    def __init__(self, nombre_archivo):
        """
        Constructor: se ejecuta automáticamente al crear el objeto.
        Inicializa el nombre del archivo y lo abre en modo escritura ('w').
        """
        self.nombre = nombre_archivo
        try:
            self.archivo = open(self.nombre, 'w')
            print(f"[INFO] Archivo '{self.nombre}' abierto correctamente.")
        except Exception as e:
            print(f"[ERROR] No se pudo abrir el archivo: {e}")

    def escribir(self, texto):
        """
        Método para escribir texto en el archivo.
        :param texto: texto a escribir.
        """
        if hasattr(self, 'archivo') and self.archivo:
            self.archivo.write(texto + '\n')
            print(f"[INFO] Texto escrito en el archivo '{self.nombre}'.")

    def __del__(self):
        """
        Destructor: se ejecuta automáticamente al destruir el objeto.
        Cierra el archivo si está abierto.
        """
        if hasattr(self, 'archivo') and self.archivo:
            try:
                self.archivo.close()
                print(f"[INFO] Archivo '{self.nombre}' cerrado correctamente.")
            except Exception as e:
                print(f"[ERROR] No se pudo cerrar el archivo: {e}")


# Código de prueba (puedes eliminarlo si solo deseas la clase)
if __name__ == "__main__":
    archivo1 = Archivo("ejemplo.txt")  # Crea el objeto y abre el archivo
    archivo1.escribir("Este es un ejemplo de uso de constructores y destructores en Python.")
    archivo1.escribir("Este archivo será cerrado automáticamente.")
    # Cuando termina el programa, se destruye el objeto y se llama al destructor automáticamente
