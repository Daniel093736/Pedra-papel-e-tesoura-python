# Pedra-papel-e-tesoura-python

from time import sleep as s
from random import choice 

while True:
    jogo = str(input('\033[35m=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-\n\033[33mvamos jogar pedra papel e tesoura?\n\033[35m=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-\n'))

    if jogo == 'sim':
        print('ok, vamos jogar... \n')
        s(1)
        ppt = choice(['pedra', 'papel', 'tesoura'])
        esc = str(input('escolha "pedra, papel, ou tesoura": '))

        if esc == 'papel' and ppt == 'tesoura':
            print('cpu: {}'.format(ppt))
            print('você perdeu :( \n\n\n')

        elif esc == 'pedra' and ppt == 'papel':
            print('cpu: {}'.format(ppt))
            print('você perdeu :( \n\n\n')

        elif esc == 'tesoura' and ppt == 'pedra':
            print('cpu: {}'.format(ppt))
            print('você perdeu :( \n\n\n ')

        elif esc == ppt:
            print('cpu: {}'.format(ppt))
            print('empate \n\n\n')

        else:
            print('cpu: {}'.format(ppt))
            print('parabéns, você ganhou :)')
            break
