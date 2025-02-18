import random

def obter_dicas():
    return {
        "Mercúrio": ["Sou o menor planeta do Sistema Solar.", "Sou o mais próximo do Sol.", "Não tenho luas."],
        "Vênus": ["Sou o planeta mais quente do Sistema Solar.", "Meu dia é maior que meu ano.", "Sou chamado de estrela d'alva."],
        "Terra": ["Sou o único planeta conhecido por abrigar vida.", "Tenho um satélite natural chamado Lua.", "Sou o terceiro planeta do Sistema Solar."],
        "Marte": ["Sou chamado de planeta vermelho.", "Tenho as maiores tempestades de poeira do Sistema Solar.", "Possuo o Monte Olimpo, o maior vulcão do Sistema Solar."],
        "Júpiter": ["Sou o maior planeta do Sistema Solar.", "Tenho a Grande Mancha Vermelha, uma enorme tempestade.", "Tenho 79 luas conhecidas."]
    }

def jogo():
    dicas_dict = obter_dicas()
    planetas = list(dicas_dict.keys())
    if not planetas:
        print("Erro: Nenhum planeta disponível no jogo.")
        return
    
    planeta_escolhido = random.choice(planetas)
    dicas = dicas_dict[planeta_escolhido]
    
    print("Bem-vindo ao Jogo dos Planetas!")
    print("Tente adivinhar qual planeta estou descrevendo.")
    
    for i, dica in enumerate(dicas):
        print(f"Dica {i + 1}: {dica}")
        resposta = input("Qual é o planeta? ")
        if resposta.capitalize() == planeta_escolhido:
            print("Parabéns! Você acertou!")
            return
        else:
            print("Tente novamente!")
    
    print(f"Que pena! O planeta era {planeta_escolhido}.")

if __name__ == "__main__":
    jogo()
