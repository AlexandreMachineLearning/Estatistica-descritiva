# Estatistica-descritiva 
## Introdução aos conceitos básicos relacionados à Estatística Descritiva
Neste tópico você irá conhecer os conceitos básicos relacionados à Estatística Descritiva. 
Em Estatística Descritiva, a preocupação fundamental é a representação dos dados fazendo uso de diagramas, gráficos, além do interesse em poder resumir tais valores. Para isso é fundamental definir alguns nomes e conceitos básicos relacionados e que irá ajudar no entendimento do tópico.
### População
São todos os elementos ou indivíduos envolvidos no estudo. Exemplo: Estudantes do Ensino Médio.
### Amostra
É uma parte dos elementos da população. Exemplos: Estudantes da cidade de São Paulo no Ensino Médio.
### Parâmetro
Pode ser conceituado como uma característica da população. Exemplo: Média na disciplina de Matemática no Ensino Médio.
### Estimativa
É uma característica da amostra, que geralmente é utilizada como uma estimativa para aproximar um parâmetro.
À partir desses conceitos, você precisa entender o que é uma variável e como ela pode ser classificada.
### Variável
É a característica de um elemento da população. É utilizada uma letra maiúscula do alfabeto para representar a variável,  e uma letra minúscula para representar o valor da variável. Exemplo: X é a variável que representa a idade de um grupo de estudantes e x = 18 anos, o valor da idade desse grupo.
### Classificação das variáveis
#### Variável Qualitativa Nominal
É a variável cujos valores possíveis são atributos e não possuem hierarquia entre si. Exemplo: nacionalidade é uma variável qualitativa nominal pois não existe motivo para demonstrar superioridade entre as diversas nacionalidades.
#### Variável Qualitativa Ordinal
É a variável cujos valores são atributos numéricos e tais atributos seguem uma hierarquia entre si. Exemplo: Satisfação com atendimento é uma variável qualitativa ordinal com valores possíveis Completamente Satisfeito, Satisfeito, Insatisfeito e Completamente Insatisfeito. Dessa forma, uma satisfação completa é muito maior que uma insatisfação completa. 
#### Variável Quantitativa Discreta
É a variável cujos valores possíveis são números inteiros advindos geralmente de uma contagem. Exemplo: número de estudantes de estatística em uma sala de aula.
#### Variável Quantitativa Contínua
É a variável cujos valores possíveis pode ser qualquer número dentro de um intervalo. Exemplo: nota da avaliação de estatística.
# Exercício de fixação
## Chegou a hora de verificar o aprendizado desta seção. 
### Exercício 1 
### Uma instituição de ensino quer realizar um estudo sobre o número de irmãos dos estudantes do 3° ano do Ensino Médio e dessa forma, realizou uma pesquisa onde  40 estudantes responderam a mesma. 
#### Qual a população em estudo? Resposta: os estudantes do 3° do Ensino Médio.
#### Qual a amostra escolhida:? Resposta: 60 estudantes que responderam a pesquisa.
#### Qual a variável em estudo? Resposta: Número de irmãos de cada estudante do 3° ano
#### Classifique a variável em estudo? Resposta: É uma variável quantitativa discreta.

## Após a coleta de dados faz-se necessário a sua representação e isso deve ser feito utilizando os gráficos. A partir daqui, você vai aprender como fazer a representação dos dados através de gráficos.
## Gráficos de barras
O gráfico de barras é considerado o mais fácil de ler e entender. Podem ser representados tanto na vertical quanto na horizontal.
A título de exemplo de aplicação, mostro como criar um gráfico de barras utilizando a biblioteca matplotlib  do Python para  apresentar as notas de um grupo de 35 estudantes na disciplina de Estatística. Seguindo o código abaixo para a criação do mesmo e assista ao vídeo disponível neste link: https://youtu.be/3siG92mQX-k

# Importação da biblioteca de visualização de dados – matplotlib
import matplotlib.pyplot as plt

# Criação das variáveis x e y, onde x corresponde as notas na disciplina e y a quantidade de cada uma dessas notas.
x = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

y = [0, 0, 1, 2, 3, 6, 6, 8, 5, 2, 2]

# Criação da variável título do gráfico
titulo = “Notas em Estatística”

# Criação das variáveis referentes aos eixos x e y
eixox = “Eixo X”

eixoy = “Eixo Y”
# Criação das legendas
plt.title(titulo)

plt.xlabel(eixox)

plt.ylabel(eixoy)

plt.bar(x,y)

plt.show

# Exercício de fixação
## Chegou a hora de verificar o aprendizado desta seção. 
### Exercício 2 
### Utilizando a biblioteca matplotlib construa um gráfico de barras para representar a renda média por faixa etária para os seguintes valores:
18 - 25     1800,00
26 - 35     2450,00
36 - 45     3750,00
46 - 55     4120,00
Mais de 55  3480,00

### Gabarito
#### Importação da biblioteca de visualização de dados – matplotlib
import matplotlib.pyplot as plt
#### Criação das variáveis faixa etária e renda
faixaetaria = ['18-25', '26-35', '36-45','46-55','Mais de 55']
renda = [1800, 2450, 3750, 4120, 3480]
#### Plotagem do gráfico
plt.title('Renda média por faixa etária')

plt.xlabel('Faixa etária (anos)')

plt.ylabel('Renda média')

plt.bar(faixaetaria,renda)

plt.show


