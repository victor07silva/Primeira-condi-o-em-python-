# Primeira-condi-o-em-python-
Testando comandos em python 
# Exercício Python 28: Escreva um programa que faça o computador “pensar” em um número inteiro entre 0 e 5
# e peça para o usuário tentar descobrir qual foi o número escolhido pelo computador. O programa deverá
# escrever na tela se o usuário venceu ou perdeu.

# irei importar a biblioteca randon para pegar o numero de 0 a 5
#usei o randint para o computador escolher o numero
from random import randint
from time import sleep

#criei uma variavel int para receber o numero desejado pelo usuário
n1 = int(input('Digite um numero de 0 a 5:'))
print('PROCESSANDO...')
#Importei da biblioteca o comando sleep para fazer a maquina "pensar" para dar a resposta 
sleep(3)
#criei uma variavel para armazenar o valor aleatório que for gerado pelo comando randint
escolha = randint(0, 5)
#Usei condição para dar a alternativa de caminhos caso o usuario não acerte.. 
if n1 == escolha:
    print('PARABÉNS! VOCÊ ACERTOU O NUMERO! NUMERO:{}'.format(escolha))
else:
    print('QUE PENA, VOCÊ ERROU! NUMERO SORTEADO:{} E NUMERO ESCOLHIDO:{}'.format(escolha, n1))
