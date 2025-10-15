class Utilidades:
  @staticmethod
  def es_primo(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5) + 1):
      if n% i == 0:
          return False
    return True
@staticmethod
def es_palindromo(cadena):
   cadena = cadena.lower().replace(" ", "")
   return cadena == cadena[::-1]

@staticmethod 
def factorial(n):
   if n < 0:
       raise ValueError("NO es posible para números negativos")
   resultado = 1
    for i in range(1,n +1):
        resultado *= i
    return resultado

@staticmethod
def suma_digitos(n):
    return sum(int(digito) for digito in str(abs(n)))
  
