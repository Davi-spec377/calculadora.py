n1 = int(input("Digite um numero: "))
n2 = int(input("Digite outro numero: "))
operacao = input("Qual é a operação (+, *, /, -)? : ")

resultado = 0

match operacao:
    case '+':
        resultado = n1 + n2
        print(f"O resultado da soma entre {n1} e {n2} é: {resultado}")
    case '-':
        resultado = n1 - n2
        print(f"O resultado da subtração entre {n1} e {n2} é: {resultado}")
    case '*':
        resultado = n1 * n2
        print(f"O resultado da multiplicação entre {n1} e {n2} é: {resultado}")
    case '/':
        if n2 != 0:
            resultado = n1 / n2
            print(f"O resultado da divisão entre {n1} e {n2} é: {resultado}")
        else:
            print("Erro: Divisão por zero não é permitida.")
    case _:
        print("Por favor, digite uma operação válida (+, *, /, -).")

