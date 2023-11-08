# Anotações importantes / Desafio de Projeto DIO

Repositório para armazenar e compartilhar informações que estou aprendendo ao longo do projeto Potência Tech iFood - Desenvolvimento de Jogos, da  [Digital Inovation One](https://www.dio.me/).
# Git & GitHub
## 🧑‍💻 Comandos Importantes Git
```
 git init - Inicia o git no repositorio
 git clone <URL> - Copia repositorio remoto
 git status - Lista as modificações atuais do repositório 
 git log - Lista histórico de commits
 git add <nome-arquivo> - Adiciona o arquivo do palco(stage)
 git reset <nome-arquivo> - Remove o arquivo do palco(stage)
 git commit m"mensagem" - Realiza o commit das modificações
 git branch - Lista todas as branch locais 
 git branch <nome-da-branch> - Cria uma nova branch 
 git checkout <nome-da-branch> - Entra na branch
 git pull original <nome-da-branch> - Pucha as modificações
 git push origin <nome-da-branch> - Envia as modificações para o repositorio remoto

```


## 💾 Downloads
- [Download GIT](https://git-scm.com/downloads)
- [Download GITHUB](https://desktop.github.com/)


## 📖 Documentação
- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/)

# HTML

# CSS
- object-fit (propriedade para imagens). object-fit: fill;(padrão) ele estica ou diminui a imagem para fazer ela caber no container, porém geralmente a imagem fica distorcida. object-fit: contain; a imagem vai ser redimensionada para caber no container, sem distorcer(sem perder qualidade) porém pode nao ocupar todo o espaço do container. object-fit: cover; a imagem vai preencher todo o container, porém ao invés de ficar distorcida ela vai cortar o espaço da imagem que ultrapassar o espaço que o elemento tem, assim mantendo a qualidade da imagem, porém dependendo da imagem pode-se perder uma parte da imagem devido ao corte. object-fit: none; a imagem vai ignorar a altura e largura do elemento pai, assim tendo sua proporção de origem. object-fit: scale-down; ele vai escolher entre o countain e o none, qual das duas configurações vai ser a menor assim a aplicando. Altera a posição da img object-position: x y; podem ser %, pixels(px), left, top, center, right, bottom, etc.
- background-image: url('...'); serve para utilizar uma imagem como background (todos os formatos de imagem sao aceitos ate gifs).
- linear-gradient(purple, red) esse efeito aplica uma troca de cor no elemento, um efeito linear, idealmente usada do mesmo tom por exemplo um rosa claro e um rosa mais escuro (podem conter mais de duas cores).
- radial-gradient(purple, red) proximo do efeito linear porem em circulo.
- repeat-linear-gradient ou repeat-radial-gradient sao outras funçoes de fundo cor, listras.
- dica: da para colocar uma imagem sobre a outra.
- background-size: que pode ter como atributos : auto(automatico) vai se ajustar automaticamente ao elemento, porem se a imagem for muito grande ela nao se adapta. cover(cobrir) ocupa todo o fundo do nosso elemento mesmo se a imagem for maior ou menor que o container, porém pode ser que ela corte um pouco da imagem original para caber dentro do container, tambem perde qualidade se a diferenca de tamanho for muito grande. contain redimenciona o tamanho da imagem para fazer ela aparecer inteira, cobre a parte que conseguir. pode ser utilizado com px e % também, com um unico valor exemplo 50% define a largura, a altura sera automatica, passando dois valores ocupara largura e altura, por exemplo 200px 250px, tomar cuidado para nao esticar muito a imagem, fazendo perder qualidade.
- background-repeat essa propriedade define se a imagem deve-se repetir, verticalmente, horizontalmente, ou nao repetir, veja os atributos dessa propriedade: background-repeat: repeat; (é o comportamento padrao, fazendo a imagem se repetir na horizontal e na vertical. background-repeat: repeat-x; repete apenas na horizontal. background-repeat: repeat-y; repete apenas no eixo vertical. background-repeat: space; com esse valor a imagem vai se repitir nas duas direções tanto vertical como horizontal sem cortar a imagem e com um espaço em branco entre elas evitando corte de imagem. background-repeat: round; repete em ambos os eixos e redimenciona para caber a imagem inteira sem cortar, porem geralmente perde qualidade. background-repeat: no-repeat; faz com que a imagem nao se repita em nenhum dos eixos. Da para aplicar tambem dois atributos um para o eixo x e outro para o eixo y, por exemplo: background-repeat: round space;.
- background-position essa propriedade serve para posicionar o background, imagem, etc.. exemplos: background-position: top; / bottom, left, right, center, top left, bottom right, também pode usar px e %. Com px e % da pra separar por horizontal e vertical com dois atributos exemplo: 10px 30px; 20px 80%; left 15px; etc..

# JAVASCRIPT
## Aprendendo 
```
 - console.log('mensagem'); imprime uma mensagem
 - let variavel = 10; o let cria uma variavel que pode mudar de valor conforme desejado
 - const pi = 3.14; o const cria uma variavel de valor fixo, que nao podera ter seu valor alterado
 - operadores matemáticos = +, -, *, /.
 - operadores condicionais (booleans) = > (maior que), < (menor que), >= (maior ou igual), <= (menor ou igual), ==(igual, que ignora o tipo da variavel, podendo por exemplo ser 0 ou '0', === (igual absoluto, com  o  mesmo tipo de variavel, sem conversão implicita), && (and, e), ! (diferente de), % (resto da divisão, multiplo de).
 - fazendo comentario no código = /* (abrindo) e */ (fechando).
 - console.log(variavel.toFixed(0 a 20)) = o toFixed fixa um numerode casas decimais e arredonda, por exemplo se for passado o valor dois em um numero 36.49787856757 oque seria mostrado para o usuario seria 36.50
 - if (condicao) abre { , codigo, } fecha = (SE) somente executa as linhas de codigo do if SE as condições forem compativeis. else = (SENAO) caso o if nao seja compativel entao executa o else. else if = senao faça esse novo if . ! (negação (senao))
 - function teste() {  } = declara uma funcão de nome teste. invocando a função = teste();. return (retorna um valor).
 - objeto = é uma coleção dinamica de chaves e valor, exemplo const guilherme = { nome: 'Guilherme de lima beraldo', idade: 25 }; e para chamar a idade por exemplo seria guilherme.idade = 24; , tambem da pra deletar uma das caracteristicas por exemplo = delete guilherme.nome . Suas propriedades tambem podem receber funcoes por exemplo = idade: function() { console.log(`Minha idade é ${this.idade}`); } , o THIS significa este, entao estaria pegando o valor de idade DESTA funcao. Também é possivel acessar a propriedade dinamicamente, por exemplo a chamada normal seria console.log(guilherme.nome); e chamando dinamicamente(sem saber o nome do atributo) seria console.log(guilherme['nome']); e mudando seu valor como = guilherme['nome'] = teste; por exemplo.
 - classe = cria uma definicao de como deve ser por exemplo : class Pessoa { nome; idade; } entao as instancias podem utilizar a classe pessoa como paramento, por exemplo : const guilherme = new Pessoa(); guilherme.nome = 'guilherme beralo'; guilherme.idade = 25;
 - constructor = deixa pre definido valores que podem ser obrigatorios por exemplo: (dentro da class) constructor() { this.nome = 'teste'; this.idade = 20; } fazendo assim quando uma nova pessoa for criada ela ja tera o valor nome teste e idade 25 ja pre definidos. tambem podemos exigir que seja informado um parametro, por exemplo: constructor (nome, idade) { this.nome = nome; this.idade = idade; }
- Array (lista) exemplo : const alunos = ['Guilherme', 'Heloisa', 'Marcelo']; que estão na posição Guilherme [0], Heloisa [1], Marcelo [2]. Adicionando mais elementos no final do array(lista) = alunos.push('Valkiria'); , ou alunos[4] = 'Valkiria'; assim aplicando diretamente na posição, e para adicionar ao inicio do array(lista) alunos.unshift('Valkiria'). Também da pra sobrescrever, apagando o elemento que estiver alocado por exemplo : alunos[1] = 'João'; isso faria com que joão sobrescrevece heloisa que estava na posição 1. Removendo itens do final da lista : alunos.pop(); , para ver o elemento que foi removido: console.log(alunos.pop()); e para remover do inicio da lista alunos.shift();. Para remover mais de um item e a partir da posição que eu informar : var pos = 1; var n = 2; var itensRemovidos = vegetais.splice(pos, n);
// Isso é como se faz para remover itens, n define o número de itens a se remover,
// a partir da posição (pos) em direção ao fim da array. console.log(itensRemovidos);
// ['Nabo', 'Rabanete']
Copair um array : var copiar = frutas.slice();.
  . Acessar um item (index) do Array exemplo: var primeiro = frutas[0]; var ultimo = frutas[frutas.length - 1];. Para ver o tamanho do array(lista) = console.log(alunos.length);. Para procurar a posição de um item especifico dentro da array : const pos = frutas.indexOf("Banana"); por exemplo < . Para percorrer o array com For (estrutura de repetição), deve-se criar uma variavel para servir como index que vai ser o controlador do número de repetições a serem feitas na lista por exemplo : for(let i = 0; i < array.lenght; i++) { código } (o i++ é a mesma coisa que fazer i = i + 1, entao ele incrementa 1 no valor do index, fazendo o código seguir executando cada elemento. Separando por virgula conseguimos trabalhar com duas camadas de imagem por exemplo ou mais : background-size: 200px 100px, cover; aplicaria para duas imagens a primeira com 200px 100px e a outra com cover.



