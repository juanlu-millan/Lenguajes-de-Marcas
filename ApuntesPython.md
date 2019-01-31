# APUNTES DE PYTHON
## Cadena de caracteres
cad = "hola mundo"

cad[2:5] print(cad) te dice la parte de la cadena

cad.lower() print(cad) minuscula

cad.upper() print(cad) mayuscula

cad.title() print(cad) #primera palabra en mayuscula

cad.count("o") print(cad) #Contador

cad.count("o",5)

cad.count("o",2,5)

"o" in cad  print(cad) #Me dice si esta la letra

cad.find(la) print(cad) #Dice la posicion

cad.startswith(h) print(cad) #Te dice si empieza

cad.endswith(do) print(cad) #Te dice si termina

cad.strip() print(cad) #quitar los espacios

cad.replace("h","m").strip() #sustituyes y quita los espacios

cad.split("/") print(cad) #quita separadores (: o /)



## Listas

listas = [1,2,3]

listas2 = [1,"hola",True]

listas = []

#Para recorrer una lista
for elem in list3:
print (elem)

for i,j in zip(lista3,lista4) #te separa los valores

len(lista) #catidad de cosas

sum(lista) #suma los numeros en la lista

lista.append("A") #añade un valor

lista[0] = "A" #Cambia el contenido

sorted(lista) #Lista ordenada

del lista[3] #borra ese valor de la lista

lista.insert(1,100) #1 es la posicion y el 100 el valor añadido

lista.pop() #quita el ultimo valor y te lo muestra

lista.pop(1) #te quita el de la posicion

lista.remove(5) #quita el primer valor

lista.reverse() #pone del reves el orden de los valores

lista.index(5) #te dice la primera posicion del valor pedido

lista.count(5) #cuenta cuantos valores existen

lista =[[1,2,3][4,5,6][7,8,9]]

"for i in lista:
    for j in i:	
 	print(j)"

for palabras in range(0,num):
	nombre=input("Dime una la palabra: ")
	lista_solo.append(nombre)
	edad=int(input("Dime una edad: "))
	lista_edad.append(edad)
	lista_conjunta.append(lista_solo+lista_edad)
	del lista_solo[0]
	del lista_edad[0]

es_primo = True
numero_es_primo = int(input("Introduce un número para comprobar si es primo:"))
for num in range(2, numero_es_primo):
	if numero_es_primo % num == 0:
		es_primo = False
if es_primo:
	print("Es Primo")
else:
	print("No es Primo")


## Diccionarios

#Meter valores
dic["nombre"]="pepe"
dic["edad"]=18
dic["notas"]=[4,5,6]

print (dic["nombre"])
dic["notas"].append(7)

#Diccionarios dentro de otro
dic["Direccion"]={"Calle":"Las Botijas","num":10}
len(dic) #Longitud de el Diccionario
len(dic[nombre]) #Longitud de el elemento especificado
edad in dic #te dice la clave esta en el Diccionario

#Diccionario dentro de una lista
alumnos=[]
alumnos.append(dic)
for alumno in alumnos:
    print(alumno["nombre"])

dic3=dic2.copy() #copia diccionario
dic.clear() #vacia el diccionario
dic.update(dic2) #Añade o actuliza elementos de dos diccionarios
dic.get("nombre") o dic.get("Notas",0) #Te muestra el valor o te muestra el error que le indiques

#Nos da el error false y me mete notas en el diccionario
if not dic2.get("notas",False)
    dic2["notas"]=[]

for i in dic.keys() #lista de las claves
    print (i)

for i in dic.values() #lista de valores
    print (i)

for clave,valor in dic.items()

    print (clave,valor)

print (alumno[1]["notas"][1])

#PROGRAMACIÓN ESTRUCTURADA
def calcular.media(numero1,numero2):
    resultado=(numero1+numero2)/2
    return resultado
---------------------------------

print (calcular.media(7.2))
num1 = int(input("numero1"))
num2 = int(input("numero2"))

media = calcular_media(num1,num2)
print (media)


+++++++++++++++++++++++++++++++++

def sumar(num1,num2,num3=0):
    return num1+num2+num3

---------------------------------
a = int (input())
b = int (input())
y = sumar (a,b,5)

#recursividad
def fact(num):
    if num=1
        return 1
    else:
        return num*fact(num-1)

