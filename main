#definiendo variables
def count_vocales_consonantes(nombre):
  vocales = ['a', 'e', 'i', 'o', 'u']
  nombre = nombre.lower()
  contador_vocales = 0
  contador_consonantes = 0

  for char in nombre:
    if char.isalpha():
      if char in vocales:
        contador_vocales += 1
      else:
        contador_consonantes += 1

  return contador_vocales, contador_consonantes


#definiendo funcion de contador de letras
def most_repeated_letter(nombre):
  nombre = nombre.lower().replace(" ", "")
  letter_count = {}
  max_count = 0
  most_repeated_letters = []

  for char in nombre:
    if char.isalpha():
      if char in letter_count:
        letter_count[char] += 1
        if letter_count[char] > max_count:
          max_count = letter_count[char]
      else:
        letter_count[char] = 1

  for letter, count in letter_count.items():
    if count == max_count:
      most_repeated_letters.append(letter)

  return most_repeated_letters


# definiendo formato nombre


def formato_nombre(nombre):
  name_parts = nombre.split()
  formatted_name_parts = []

  for part in name_parts:
    formatted_name_parts.append(part.capitalize())

  return ' '.join(formatted_name_parts)


# programa
full_nombre = input("Ingrese su Nombre completo: ")
formatted_name = formato_nombre(full_nombre)
vocales, consonantes = count_vocales_consonantes(formatted_name)
must_repeated = most_repeated_letter(formatted_name)
#separated_primera_palabra = primera_palabra()

print("Separated names: ", formatted_name)
print("Nombres: ")
print("Apellidos: ")
print("Numeros de Vocales: ", vocales)
print("Numero de Consonantes: ", consonantes)

if must_repeated:
  print("Se Repiten mas las siguientes Letras: ", ', '.join(must_repeated))
else:
  print("No se repiten Letras.")
