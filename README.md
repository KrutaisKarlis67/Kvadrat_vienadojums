a = int(input("Ievadi koeficientu a: "))
b = int(input("Ievadi koeficientu b: "))
c = int(input("Ievadi koeficientu c: "))



def atrisinat_kvadratvienadojumu(a, b, c):
  
  
  if a == 0:
    return 

  D = b**2 - 4 * a * c

  print(f"Diskriminants D = {b}^2 - 4 * {a} * {c} = {D}")

  if D > 0:

    x1 = (-b + D**0.5) / (2 * a)
    x2 = (-b - D**0.5) / (2 * a)
    return f"Vienādojumam ir divas saknes: x1 = {x1}, x2 = {x2}"

  elif D == 0:
  
    x = -b / (2 * a)
    return f"Vienādojumam ir viena sakne: x = {x}"

  else:
    
    return "Diskriminants ir negatīvs (D < 0), tāpēc reālo sakņu nav."




rezultats = atrisinat_kvadratvienadojumu(a, b, c)
print(rezultats)
