class Persona:
    def __init__(self, nombre, edad, pronombres, genero, peliculas_favoritas, mbti):
        self.nombre = nombre
        self.edad = edad
        self.pronombres = pronombres
        self.genero = genero
        self.peliculas_favoritas = peliculas_favoritas
        self.mbti = mbti
    
    def presentar(self):
        # Presentación detallada de la persona
        print(f"Hola, me llamo {self.nombre}.")
        print(f"Tengo {self.edad} años.")
        print(f"Mis pronombres son {self.pronombres}.")
        print(f"Me identifico como {self.genero}.")
        print("Mis películas favoritas son:")
        for pelicula in self.peliculas_favoritas:
            print(f" - {pelicula}")
        print(f"Mi tipo de personalidad MBTI es {self.mbti}.")

# Ejemplo de uso:
persona1 = Persona(
    nombre="Piero",
    edad=18,
    pronombres="él",
    genero="masculino",
    peliculas_favoritas=["Requiem for a Dream", "Dancer in the Dark", "Blade Runner"],
    mbti="INTP"
)

persona1.presentar()
