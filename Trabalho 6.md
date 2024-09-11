**Primeiro exercício** 
def imprimir_informacoes(nome, idade, cidade):
    # Usar o argumento sep para adicionar "- " entre as informações
    print(f"Nome: {nome}", end=" - ")
    print(f"Idade: {idade}", end=" - ")
    print(f"Cidade: {cidade}")

# Exemplo de uso
imprimir_informacoes("Helena", 23, "Rio de Janeiro")



**Segundo exercício** 
def calculadora():
    # Pedir ao usuário para inserir o primeiro número
    num1 = float(input("Digite o primeiro número: "))
    
    # Pedir ao usuário para inserir o segundo número
    num2 = float(input("Digite o segundo número: "))
    
    # Pedir ao usuário para inserir a operação desejada
    operacao = input("Digite a operação desejada (+, -, *, /): ")
    
    # Verificar qual operação foi escolhida e calcular o resultado
    if operacao == '+':
        resultado = num1 + num2
    elif operacao == '-':
        resultado = num1 - num2
    elif operacao == '*':
        resultado = num1 * num2
    elif operacao == '/':
        # Verificar se o divisor é zero para evitar divisão por zero
        if num2 != 0:
            resultado = num1 / num2
        else:
            print("Erro: Divisão por zero não é permitida.")
            return
    else:
        print("Operação inválida. Use +, -, * ou /.")
        return
    
    # Imprimir o resultado
    print(f"O resultado de {num1} {operacao} {num2} é {resultado}")

# Chamar a função para executar
calculadora()


**Terceiro exercício**
def listar_compras():
    # Pedir ao usuário para inserir itens da lista de compras separados por vírgula
    itens = input("Digite os itens da lista de compras, separados por vírgula: ")
    
    # Dividir a string em uma lista de itens, removendo espaços extras
    lista_compras = [item.strip() for item in itens.split(',')]
    
    # Imprimir os itens numerados
    for i, item in enumerate(lista_compras, start=1):
        print(f"Item {i}: {item}")

# Chamar a função para executar
listar_compras()


**Quarto Exercício** 
def converter_celsius_para_fahrenheit():
    # Solicitar ao usuário a temperatura em graus Celsius
    celsius = float(input("Digite a temperatura em graus Celsius: "))
    
    # Converter a temperatura de Celsius para Fahrenheit
    fahrenheit = (celsius * 9/5) + 32
    
    # Imprimir o resultado
    print(f"A temperatura em Fahrenheit é: {fahrenheit:.2f}")

# Chamar a função para executar
converter_celsius_para_fahrenheit()


**Quinto exercício**
def coletar_nomes():
    nomes = []  # Lista para armazenar os nomes digitados
    
    while True:
        # Solicitar ao usuário que digite um nome
        nome = input("Digite um nome (ou 'sair' para encerrar): ")
        
        # Verificar se o nome digitado é 'sair'
        if nome.lower() == 'sair':
            break
        
        # Adicionar o nome à lista
        nomes.append(nome)
    
    # Imprimir todos os nomes, cada um em uma linha
    print("\nNomes digitados:")
    for nome in nomes:
        print(nome)

# Chamar a função para executar
coletar_nomes()
