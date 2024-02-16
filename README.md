# modelo-calculadora-de-porcentagem
Calcula a porcentagem desejada em cima do valor desejado


n = True

try:    
    while n == True:
    
        preço = float(input('Qual preço do produto: '))
        imposto = int(input('Qual a porcentagem de imposto? [1] a [100]: '))

        novo_imposto = (imposto / 100) 

        imposto_a_ser_pago = preço * novo_imposto

        print(f'A porcentagem de imposto é de {novo_imposto}% e o valor a ser pago é de R${imposto_a_ser_pago}!')
    
        deseja_continuar = input('Deseja continuar? [S]IM / [N]ÃO: ').upper().strip()
        if deseja_continuar == 'S':
            continue
        else:
            break
        
except:
    print('Porcentagem inexistente escolha entre [1%] e [100%]')
