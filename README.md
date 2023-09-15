# UnB.oo
# Função para calcular a área de um círculo
def calcular_area_circulo(raio):
    return 3.14159 * raio ** 2

# Função para calcular a área de um retângulo
def calcular_area_retangulo(base, altura):
    return base * altura

# Função para calcular a área de um triângulo
def calcular_area_triangulo(base, altura):
    return 0.5 * base * altura

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
        area = calcular_area_circulo(raio)
        formas.append(("círculo", area))
        print(f"Círculo com raio {raio} adicionado com sucesso.")

    elif escolha == "2":
        base = float(input("Digite a base do retângulo: "))
        altura = float(input("Digite a altura do retângulo: "))
        area = calcular_area_retangulo(base, altura)
        formas.append(("retângulo", area))
        print(f"Retângulo com base {base} e altura {altura} adicionado com sucesso.")

    elif escolha == "3":
        base = float(input("Digite a base do triângulo: "))
        altura = float(input("Digite a altura do triângulo: "))
        area = calcular_area_triangulo(base, altura)
        formas.append(("triângulo", area))
        print(f"Triângulo com base {base} e altura {altura} adicionado com sucesso.")

    elif escolha == "4":
        area_total = sum(area for _, area in formas)
        print(f"A área total das formas é: {area_total}")

    elif escolha == "5":
        print("Encerrando o programa.")
        break

    else:
        print("Opção inválida. Por favor, escolha uma opção válida.")