# Definir a classe Circle para representar círculos
class Circle:
    def __init__(self, radius):
        self.radius = radius

    def calcular_area(self):
        return 3.14159 * self.radius ** 2

# Definir a classe Rectangle para representar retângulos
class Rectangle:
    def __init__(self, base, altura):
        self.base = base
        self.altura = altura

    def calcular_area(self):
        return self.base * self.altura

# Definir a classe Triangle para representar triângulos
class Triangle:
    def __init__(self, base, altura):
        self.base = base
        self.altura = altura

    def calcular_area(self):
        return 0.5 * self.base * self.altura

# Inicializar uma lista vazia para armazenar as formas
formas = []

# Loop interativo
while True:
    print("Escolha uma opção:")
    print("1. Adicionar círculo")
    print("2. Adicionar retângulo")
    print("3. Adicionar triângulo")
    print("4. Calcular área total")
    print("5. Sair")

    escolha = input("Digite o número da opção: ")

    if escolha == "1":
        raio = float(input("Digite o raio do círculo: "))
        forma = Circle(raio)
        formas.append(forma)
        print(f"Círculo com raio {raio} adicionado com sucesso.")

    elif escolha == "2":
        base = float(input("Digite a base do retângulo: "))
        altura = float(input("Digite a altura do retângulo: "))
        forma = Rectangle(base, altura)
        formas.append(forma)
        print(f"Retângulo com base {base} e altura {altura} adicionado com sucesso.")

    elif escolha == "3":
        base = float(input("Digite a base do triângulo: "))
        altura = float(input("Digite a altura do triângulo: "))
        forma = Triangle(base, altura)
        formas.append(forma)
        print(f"Triângulo com base {base} e altura {altura} adicionado com sucesso.")

    elif escolha == "4":
        area_total = sum(forma.calcular_area() for forma in formas)
        print(f"A área total das formas é: {area_total}")

    elif escolha == "5":
        print("Encerrando o programa.")
        break

    else:
        print("Opção inválida. Por favor, escolha uma opção válida.")
