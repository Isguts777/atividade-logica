# Criação da matriz 3x3
matriz = [[], [], []]

for i in range(3):
    for j in range(3):
        valor = int(input(f'Digite um valor para [{i}, {j}]: '))
        matriz[i].append(valor)

# Exibicao
print('\nMatriz digitada:')
for linha in matriz:
    for elemento in linha:
        print(f'[ {elemento:^5} ]', end=' ')
    print()

# A) Soma
soma_pares = 0
for linha in matriz:
    for elemento in linha:
        if elemento % 2 == 0:
            soma_pares += elemento

# B) Soma 
soma_terceira_coluna = matriz[0][2] + matriz[1][2] + matriz[2][2]

# C) soma
maior_segunda_linha = max(matriz[1])

# Exibir resultados
print(f'\nA) Soma dos valores pares: {soma_pares}')
print(f'B) Soma dos valores da terceira coluna: {soma_terceira_coluna}')
print(f'C) Maior valor da segunda linha: {maior_segunda_linha}')
