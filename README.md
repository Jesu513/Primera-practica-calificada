# Primera-practica-calificada
# Ejercicio 1

    def Fibonacci(N):
    
       if(N==0):
        
          return 0
    
       elif(N==1):
        
          return 1
    
       else:
        
          return (Fibonacci(N-2)+Fibonacci(N-1)) 

    n=int(input("ingrese un numero 'n': "))

    print("la secuencia de fibonacci es: ")

    for n in range(0, n+1):
  
         print(Fibonacci(n))

# Ejercicio 3

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

# Ejercicio 4

    def mcd(M,N):
    
        if M==N:
        
           m=M
    
        elif M>N:
        
           m=mcd(M-N,N)
    
        else:
        
           m=mcd(N,M%N)
    
        return m

    M=int(input("Ingrese el primer número: "))

    N=int(input("Ingrese el primer número: "))

    print(f"El maximo divisor es {mcd(M,N)}")

# Ejercicio 5

    def entero_a_binario(num):

       if num == 0:
        
          return ""
    
       else:
        
          return str(num % 2) + entero_a_binario(num // 2)

    print(entero_a_binario(5))

    print(entero_a_binario(7))
   
 # Ejercicio 6
   
    def moverTorre(altura, origen, destino, intermedio):
    
       if altura >= 1:
        
          moverTorre(altura - 1, origen, intermedio, destino)
        
          moverDisco(origen, destino)
        
          moverTorre(altura - 1, intermedio, destino, origen)


    def moverDisco(desde, hacia):
     
       print("mover disco de", desde, "a", hacia)


    moverTorre(3, "A", "B", "C")
