# provaAlgHj

REPETIÇÂO

1 ⦁	Faça um algoritmo que soma os números de 1 a 100 e exibe resultado da soma

soma = 0  

for numero in range(1, 101):
    soma += numero  

print("A soma dos números de 1 a 100 é:", soma)





2⦁	Construa um Algoritmo que, para um grupo de 50 valores inteiros, determine: a) A soma dos números positivos; b) A quantidade de valores negativos

soma_positivos = 0
quantidade_negativos = 0


for i in range(50):
    valor = int(input(f"Digite o {i + 1}º valor inteiro: "))
    
    if valor > 0:
        soma_positivos += valor
    elif valor < 0:
        quantidade_negativos += 1

print("Soma dos números positivos:", soma_positivos)
print("Quantidade de valores negativos:", quantidade_negativos)





3 ⦁	Faça um algoritmo que imprima os múltiplos positivos de 7, inferiores a 1000.

for numero in range(1, 1000):
    if numero % 7 == 0:
        print(numero)






        
4⦁	⦁	Faça um algoritmo que calcule a média de salários de uma empresa, pedindo ao usuário a quantidade de funcionários, o nome e o salário de cada funcionário e devolvendo a média, o salário mais alto e o salário mais baixo


num_funcionarios = int(input("Digite a quantidade de funcionários: "))


soma_salarios = 0
salario_mais_alto = float('-inf')  
salario_mais_baixo = float('inf')  


for i in range(num_funcionarios):
    nome = input(f"Digite o nome do funcionário {i + 1}: ")
    salario = float(input(f"Digite o salário do funcionário {i + 1}: "))
    
   
    soma_salarios += salario
    
   
    if salario > salario_mais_alto:
        salario_mais_alto = salario
    if salario < salario_mais_baixo:
        salario_mais_baixo = salario


media_salarios = soma_salarios / num_funcionarios


print(f"A média dos salários é: {media_salarios:.2f}")
print(f"O salário mais alto é: {salario_mais_alto:.2f}")
print(f"O salário mais baixo é: {salario_mais_baixo:.2f}")




5 ⦁	Escreva um algoritmo que determine o fatorial de um número. Para este problema, tem-se como entrada o valor do número do qual se deseja calcular o fatorial. O fatorial de 0 é igual a 1. O fatorial de um número N(N!) é definido conforme a seguir:
N! = 1 * 2 * 3 * 4 * ... * (N-1) * N

numero = int(input("Digite um número inteiro não negativo: "))


fatorial = 1

if numero < 0:
    print("O fatorial não está definido para números negativos.")
elif numero == 0:
    print("O fatorial de 0 é 1.")
else:

    for i in range(1, numero + 1):
        fatorial *= i

    
    print(f"O fatorial de {numero} é {fatorial}.")



6  

⦁	 Sem utilizar a operação de multiplicação, escreva um programa que multiplique dois números inteiros. Por exemplo: 2 * 2 = 2 + 2.
⦁	 



numero1 = int(input("Digite o primeiro número inteiro: "))
numero2 = int(input("Digite o segundo número inteiro: "))


resultado = 0


for _ in range(abs(numero2)):
    resultado += numero1


if numero1 < 0 and numero2 > 0:
    resultado = -resultado
elif numero1 > 0 and numero2 < 0:
    resultado = -resultado


print(f"O resultado da multiplicação é: {resultado}")




7 A série de Fibonacci é formada pela sequência: 0, 1, 1, 2, 3, 5, 8, 13, 21, ... Construa um algoritmo que gere e mostre a série até o vigésimo termo.


termo1 = 0
termo2 = 1


print(termo1)
print(termo2)


for i in range(18):
    proximo_termo = termo1 + termo2
    print(proximo_termo)
    
   
    termo1 = termo2
    termo2 = proximo_termo




8 ⦁	Faça um algoritmo que leia um conjunto de números (X) e imprima sua soma (Soma) e sua média (Media). Admita que o valor 9999 é utilizado como sentinela para fim de leitura. Ex.: 1, 2, 3 => Soma=6 Media=2


soma = 0
contador = 0


while True:
    numero = int(input("Digite um número (ou 9999 para encerrar): "))
    
    if numero == 9999:
        break  
    else:
        soma += numero
        contador += 1


if contador == 0:
    media = 0
else:
    media = soma / contador


print(f"Soma = {soma}")
print(f"Média = {media}")



9 ⦁	Escrever um algoritmo que lê um valor N inteiro e positivo e que calcula e escreve o valor de E. E = 1 + 1 / 1! + 1 / 2! + 1 / 3! + 1 / N!


N = int(input("Digite um valor inteiro e positivo para N: "))


E = 1


fatorial = 1


for i in range(1, N + 1):
    fatorial *= i  
    termo = 1 / fatorial  
    E += termo  


print(f"O valor de E é aproximadamente: {E:.6f}")








 

