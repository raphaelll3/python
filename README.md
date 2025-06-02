# python

# Criação do dicionário para armazenar os produtos e preços
produtos = {}

# Solicitação dos dados ao usuário
for i in range(5):
    nome = input(f"Digite o nome do produto {i + 1}: ")
    while True:
        try:
            preco = float(input(f"Digite o preço do produto '{nome}': R$ "))
            break
        except ValueError:
            print("Por favor, insira um valor numérico válido.")
    produtos[nome] = preco

# Cálculo do valor total da compra
valor_total = sum(produtos.values())

# Exibição do resultado
print("\nResumo da Compra:")
for nome, preco in produtos.items():
    print(f"- {nome}: R$ {preco:.2f}")
print(f"\nValor total da compra: R$ {valor_total:.2f}")























