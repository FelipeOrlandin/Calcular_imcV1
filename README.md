# Calcular_imcV1
A ideia é calcular o imc da pessoa e informar se ela esta acima abaixo ou no peso ideal /
The idea is to calculate the person's BMI and tell if they are above, below or at the ideal weight
#

nome = input('Informe seu nome: ')

idade = input('Informe sua idade: ')

altura = input("Informe sua altura: ")

peso = input('Informe seu peso: ')

ano_atual = input('Informe ano atual: ')

peso_f = float(peso)

altura_f = float(altura)

ano_atual = int(ano_atual)

idade = int(idade)

nascimento = ano_atual - idade

imc = peso_f / altura_f ** 2

print(f'=============================================')

print(f'{nome} tem {idade} anos e {altura} de altura.')

print(f'{nome} pesa {peso} e seu imc é {imc:.2f}.')

print(f'{nome} nasceu em {nascimento}')

print()


if imc <= 18.9:
    print(f'{nome} Você esta abaixo do peso' )

if imc >= 19 and imc <= 24.9:
    print(f'{nome} Você esta no peso ideal')

if imc >= 25:
    print(f'{nome} Você esta com sobrepeso')

print(f'=============================================')

