# pythonProjectRPG
Atividade avaliativa POO criando um jogo de rpg
#Criando a classe "Personagem",
class Personagem:
    def __init__(self, nome, classe, nivelexperiencia):
        self.nome = nome
        self.classe = classe
        self.nivelexperiencia = nivelexperiencia
    #definindo as ações que podem ser feito pelas personagens
    def atacar(self):
            print(self.nome, self.classe, self.nivelexperiencia, str("ataca seu oponente"))
    def defender(self):
            print(self.nome, self.classe, self.nivelexperiencia, str("defende do ataque de seu oponente"))
    def ultimate(self):
            print(self.nome, self.classe, self.nivelexperiencia, str("utiliza sua ultimate"))

#Criando a classe Guerreiro que herda da classe Personagem
class Guerreiro(Personagem):
    def __init__(self, nome, classe, nivelexperiencia):
        super().__init__(nome, "Guerreiro", nivelexperiencia)
#criando a classe Mago que também herda da classe Personagem
class Mago(Personagem):
    def __init__(self, nome, classe, nivelexperiencia):
        super().__init__(nome, "Mago", nivelexperiencia)
#criando a classe Atirador herdando a classe Personagem
class Atirador(Personagem):
    def __init__(self, nome, classe, nivelexperiencia):
        super().__init__(nome, "Atirador", nivelexperiencia)
#criando também a classe Assassino que herda também da Classe Personagem
class Assassino(Personagem):
    def __init__(self, nome, classe, nivelexperiencia):
        super().__init__(nome, "Assassino", nivelexperiencia)
#instanciando objetos as classes guerreiro, mago, atirador e assassino, definindo seu nome sua classe e seu nivel de experiência.
guerreiro = Guerreiro("Leonard", "Guerreiro", 7)

mago = Mago("Violet", "Mago", 9)

atirador = Atirador("Roberto", "Atirador", 6)

assassino = Assassino("Eduardo", "Assassino", 8)
#Chamando os métodos atacar, defender e ultimate nas classes guerreiro, mago, atirador e assassino.
guerreiro.atacar()

mago.atacar()

atirador.atacar()

assassino.atacar()

mago.defender()

atirador.defender()

guerreiro.ultimate()

assassino.defender()

guerreiro.ultimate()

mago.ultimate()

atirador.ultimate()

assassino.ultimate()
#finalizando a batalha com uma mensagem fina!
print("Parabéns, todos os oponente foram derrotados!")
