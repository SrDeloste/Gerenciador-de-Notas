#solicitando as informações para o usuario
nome_aluno = input('Digite o nome do aluno: ')
p1 = float(input('Digite a nota da primeira prova:'))
p2 = float(input('Digite o nota da segunada prova:'))
# Pergunta se há mais de uma atividade
resposta = input('Tem mais de uma atividade? (sim/não): ')

if resposta.lower() == 'sim':
    # Se a resposta for sim, pergunte quantas atividades
    num_atividades = int(input('Quantas atividades? '))

    if num_atividades > 2:
        # Se houver mais de duas atividades, calcule todas
        soma = 0
        for i in range(num_atividades):
            nota = float(input(f'Digite a nota da atividade {i + 1}: '))
            soma += nota
        media = soma / num_atividades
    else:
        # Se houver duas ou menos atividades, calcule a média
        soma = 0
        for i in range(num_atividades):
            nota = float(input(f'Digite a nota da atividade {i + 1}: '))
            soma += nota
        media = soma / num_atividades
else:
    # Se a resposta for não, calcule uma atividade
    nota = float(input('Digite a nota da atividade: '))
    media = nota

#Calculando a media final 
media_final = ((p1 + p2) / 2) * (0.8 + 0.04 * num_atividades)
#Verificando a situação do aluno 
if media_final> 10:
    media_final = 10
if media_final >= 6:
    situacao = "Aprovado"
    mensagem_situacao = "Parabéns! Você foi aprovado."
elif media_final < 5:
    situacao = "Reprovado"
    mensagem_situacao = "Infelizmente você foi reprovado. Estude mais na próxima vez."
else:
    situacao = "Recuperação"
    mensagem_situacao = "Você está de recuperação. Continue se esforçando para melhorar sua média."
    
print('A média das atividades é: {media:.2f}')
print("\nResultado:")
print(f"Nome do aluno: {nome_aluno}")
print(f"Nota da P1: {p1:.2f}")
print(f"Nota da P2: {p2:.2f}")
print(f"Nota das atividades (ATV): {num_atividades:.2f}")
print(f"Média final: {media_final:.2f}")
print(f"Situação: {situacao}\n{mensagem_situacao}")
