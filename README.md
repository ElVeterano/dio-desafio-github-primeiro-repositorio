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
 - objeto = é uma coleção dinamica de chaves e valor, exemplo const guilherme = { nome: 'Guilherme de lima beraldo', idade: 25 }; e para chamar a idade por exemplo seria guilherme.idade = 24; , tambem da pra deletar uma das caracteristicas por exemplo = delete guilherme.nome . Suas propriedades tambem podem receber funcoes por exemplo = idade: function() { console.log('Minha idade é ${this.idade}'); } , o THIS significa este, entao estaria pegando o valor de idade DESTA funcao. Também é possivel acessar a propriedade dinamicamente, por exemplo a chamada normal seria console.log(guilherme.nome); e chamando dinamicamente(sem saber o nome do atributo) seria console.log(guilherme['nome']); e mudando seu valor como = guilherme['nome'] = teste; por exemplo.
 - classe = cria uma definicao de como deve ser por exemplo : class Pessoa { nome; idade; } entao as instancias podem utilizar a classe pessoa como paramento, por exemplo : const guilherme = new Pessoa(); guilherme.nome = 'guilherme beralo'; guilherme.idade = 25;
 - constructor = deixa pre definido valores que podem ser obrigatorios por exemplo: (dentro da class) constructor() { this.nome = 'teste'; this.idade = 20; } fazendo assim quando uma nova pessoa for criada ela ja tera o valor nome teste e idade 25 ja pre definidos.
