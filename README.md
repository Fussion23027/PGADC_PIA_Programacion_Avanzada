# Ejercicio a, b y c
class TDevice:
    def __init__(self, tamaño, peso, altura, marca):
        self.tamaño = tamaño
        self.peso = peso
        self.altura = altura
        self.marca = marca

    def encender(self):
        print("Encendiendo dispositivo")

    def apagar(self):
        print("Apagando dispositivo")

class TV(TDevice):
    def cambiar_canal(self, canal):
        print(f"Cambiando al canal {canal}")

    def ajustar_volumen(self, volumen):
        print(f"Ajustando el volumen a {volumen}")

class Licuadora(TDevice):
    def mezclar(self, velocidad):
        print(f"Mezclando a velocidad {velocidad}")

    def triturar(self, tiempo):
        print(f"Triturando por {tiempo} segundos")

class Celular(TDevice):
    def llamar(self, numero):
        print(f"Llamando al número {numero}")

    def enviar_mensaje(self, mensaje):
        print(f"Enviando mensaje: {mensaje}")


tv1 = TV("Grande", "5kg", "50cm", "Samsung")
tv2 = TV("Pequeña", "3kg", "30cm", "LG")

licuadora1 = Licuadora("Mediana", "2kg", "40cm", "Oster")
licuadora2 = Licuadora("Grande", "4kg", "50cm", "Hamilton Beach")

celular1 = Celular("Pequeño", "0.2kg", "15cm", "Apple")
celular2 = Celular("Mediano", "0.3kg", "16cm", "Samsung")


tv1.cambiar_canal(5)
licuadora1.mezclar(3)
celular1.llamar(3)


# Ejercicio d, e, f y g
class PersonaC:
    def __init__(self,nombre,edad,genero,altura,peso):
       self.nombre= nombre
       self.edad = edad
       self.genero = genero
       self.altura = altura
       self.peso = peso


class Policia (PersonaC):
    def arrestar (self):
        print(f"Arrestado el sospechoso {self.nombre}")
        print("Datos de la policia")
        print("Nombre: ",self.nombre)
        print("Edad: ", self.edad)
        print("Genero: ",self.genero)
        print("Altura: ",self.altura)
        print("Peso: ",self.peso)


        print("-------------------------------------------------------------------------------------")
        print("-------------------------------------------------------------------------------------")
class Administrador (PersonaC):
    def atender (self):
        print(f"Usuario Atendido {self.nombre}")
        print("Datos del Administrador")
        print("Nombre: ",self.nombre)
        print("Edad: ", self.edad)
        print("Genero: ",self.genero)
        print("Altura: ",self.altura)
        print("Peso: ",self.peso)


        print("-------------------------------------------------------------------------------------")
        print("-------------------------------------------------------------------------------------")
class Bombero (PersonaC):
    def incendio (self):
        print(f"Usuario Antendido por llamas {self.nombre}")
        print("Datos de la Bomberos")
        print("Nombre: ",self.nombre)
        print("Edad: ", self.edad)
        print("Genero: ",self.genero)
        print("Altura: ",self.altura)
        print("Peso: ",self.peso)


policia_estacion_1=Policia("Pablo",29,"Masculino",1.70,'70kg')
ambulancia_estacion_1=Administrador("Maria",30,"Femenino",1.80,'50kg')
bombero_estacion_1=Bombero("Lopez",28,"Masculino",1.90,'80kg')


policia_estacion_1.arrestar()
ambulancia_estacion_1.atender()
bombero_estacion_1.incendio()



# Ejercicio h
class Personas:
  def __init__(self, nombre, edad, genero):
    self.nombre= nombre
    self.edad= edad
    self.genero= genero

  def presentarse(self):
    print(f"Hola me presento soy {self.nombre} y tengo {self.edad} años")

#Ejercicio  i

class Estudiante (Personas):
  def  __init__(self, nombre, edad, genero , curso):
    self.nombre = nombre
    self.edad= edad
    self.genero= genero
    self.curso= curso

  def estudiar(self):
      print(f"Estoy estudiando el curso  de {self.curso}.")

# Ejercicio J

class  Rectangulo:
    def __init__(self, largo, ancho):
       self.largo = largo
       self.ancho = ancho
    def area(self):
       return  self.largo * self.ancho
rectangulo = Rectangulo(5,3)
print("El area del rectangulo es: ", rectangulo.area())
