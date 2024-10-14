#Diccionario 
#Los diccionarios se utilizan para almacenar valores de datos en pares clave:valor.

#Un diccionario es una colección ordenada*, modificable y que no permite duplicados.

#1- Creando y desplegando diccionario

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)


#2- Imprima el valor de "brand" o "marca"  del diccionario:
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])


#4- Los valores duplicados sobrescribirán los valores existentes:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964,
  "year": 2020
}
print(thisdict)


#Imprima la cantidad de elementos en el diccionario:

#5- Print the number of items in the dictionary:
print(len(thisdict))


#6- Tipos de datos de cadena, int, booleanos y de lista:
thisdict = {
  "brand": "Ford",
  "electric": False,
  "year": 1964,
  "colors": ["red", "white", "blue"]
}

#7-  Imprima el tipo de datos de un diccionario:
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(type(thisdict))


#8-  Usando el método dict() para hacer un diccionario:
thisdict = dict(name = "John", age = 36, country = "Norway")
print(thisdict)

print("");print("practicando");print("")
c={}
def a(n,t):
    c[n] = t
    print(f"Contacto {n} agregado.")
def e(n):
    if n in c:
        del c[n]
        print(f"Contacto {n} eliminado.")
    else:
        print(f"Contacto {n} no encontrado.")
def b(n):
    if n in c:
        print(f"{n}: {c[n]}")
    else:
        print(f"Contacto {n} no encontrado.")
while True:
    print("\nGestión de Contactos")
    print("1. Agregar contacto")
    print("2. Eliminar contacto")
    print("3. Buscar contacto")
    print("4. Salir");print("")
    o=input("Elige una opción: ")
    if o=="1":
        n=input("Nombre: ")
        t=input("Teléfono: ")
        a(n,t)
    elif o=="2":
        n=input("Nombre: ")
        e(n)
    elif o=="3":
        n=input("Nombre: ")
        buscar_contacto(n)
    elif o=="4":
        print("Saliendo del programa...")
        break
    else:
        print("Opción no válida. Inténtalo de nuevo.")

        ![image](https://github.com/user-attachments/assets/3b051533-04b2-4efa-bfd4-15e5282e7359)
        ![image](https://github.com/user-attachments/assets/800dc60e-b63e-4469-8c6a-dd6617e2c3ab)
