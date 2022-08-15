# Primera-practica-calificada
def ent(a):
  if a==0:
    r=a
  elif a==1:
    r=a
  else:
    r=(a*(a+1))//2
  return r

a=int(input("Ingrese un número: "))
print("La suma de los primeros N enteros es: ",ent(a))
