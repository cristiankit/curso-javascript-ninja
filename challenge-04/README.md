# Desafio da semana #4

```js
/*
Declare uma variável chamada `isTruthy`, e atribua a ela uma função que recebe
um único parâmetro como argumento. Essa função deve retornar `true` se o
equivalente booleano para o valor passado no argumento for `true`, ou `false`
para o contrário.
*/
var isTruthy = function(a){
	var teste;
	if(a){teste = true;}else{teste = false;};
	return teste;
}
// ou
var isTruthy = function(a){
	return !! a;
}

// Invoque a função criada acima, passando todos os tipos de valores `falsy`.
isTruthy();
isTruthy("");
isTruthy(0);
isTruthy(-0);
isTruthy(NaN);
isTruthy(false);






/*
Invoque a função criada acima passando como parâmetro 10 valores `truthy`.
*/
isTruthy(1);
isTruthy("kit");
isTruthy(true);
isTruthy("zeca");
isTruthy(5);
isTruthy(6);
isTruthy("kitDrums");
isTruthy("0");
isTruthy("1");
isTruthy("-0");
isTruthy("NaN");
isTruthy("false");

/*
Declare uma variável chamada `carro`, atribuindo à ela um objeto com as
seguintes propriedades (os valores devem ser do tipo mostrado abaixo):
- `marca` - String
- `modelo` - String
- `placa` - String
- `ano` - Number
- `cor` - String
- `quantasPortas` - Number
- `assentos` - Number - cinco por padrão
- `quantidadePessoas` - Number - zero por padrão
*/
var carro = {};
carro.ano =  "2020";
carro.assentos = 5;
carro.cor = "azul";
carro.marca = "gol";
carro.modelo = "2019";
carro.placa = "12445WW";
carro.quantasPortas = 4;
carro.quantidadePessoas = 0;

/*
Crie um método chamado `mudarCor` que mude a cor do carro conforme a cor
passado por parâmetro.
*/
var mudaCor = function(cor){
	carro.cor = cor;
}

/*
Crie um método chamado `obterCor`, que retorne a cor do carro.
*/
var obterCor = function(){
	return carro.cor;
}

/*
Crie um método chamado `obterModelo` que retorne o modelo do carro.
*/
var obterModelo = function(){
  return carro.modelo;
};

/*
Crie um método chamado `obterMarca` que retorne a marca do carro.
*/
var obterMarca = function(){
  return carro.marca;
};

/*
Crie um método chamado `obterMarcaModelo`, que retorne:
"Esse carro é um [MARCA] [MODELO]"
Para retornar os valores de marca e modelo, utilize os métodos criados.
*/
var obterMarcaModelo = function(){
  return "Esse carro é um " + carro.marca + " " + carro.modelo + ""
};

/*
Crie um método que irá adicionar pessoas no carro. Esse método terá as
seguintes características:
- Ele deverá receber por parâmetro o número de pessoas entrarão no carro. Esse
número não precisa encher o carro, você poderá acrescentar as pessoas aos
poucos.
- O método deve retornar a frase: "Já temos [X] pessoas no carro!"
- Se o carro já estiver cheio, com todos os assentos já preenchidos, o método
deve retornar a frase: "O carro já está lotado!"
- Se ainda houverem lugares no carro, mas a quantidade de pessoas passadas por
parâmetro for ultrapassar o limite de assentos do carro, então você deve
mostrar quantos assentos ainda podem ser ocupados, com a frase:
"Só cabem mais [QUANTIDADE_DE_PESSOAS_QUE_CABEM] pessoas!"
- Se couber somente mais uma pessoa, mostrar a palavra "pessoa" no retorno
citado acima, no lugar de "pessoas".
*/
var adicionarPessoasnoCarro = funtion(numeroDePessoas){
  var numeroDePessoas = "Já temos " + numeroDePessoas + " pessoas no carro!";
  var carroCheio = "O carro já está lotado!";
  var numeroDeAssentos = "Só cabem mais " + carro.quantidadePessoas + pessoasSingular + "!";
  var pessoasSingular = "pessoas";
  if(carro.quantidadePessoas >= carro.assentos){carroCheio};
  if(carro.quantidadePessoas <= carro.assentos-1 && numeroDePessoas > carro.assentos){numeroDeAssentos};
  if(carro.quantidadePessoas === 4){
  pessoasSingular = "pessoa";
  return numeroDeAssentos;
};
};

/*
Agora vamos verificar algumas informações do carro. Para as respostas abaixo,
utilize sempre o formato de invocação do método (ou chamada da propriedade),
adicionando comentários _inline_ ao lado com o valor retornado, se o método
retornar algum valor.

Qual a cor atual do carro?
*/
?

// Mude a cor do carro para vermelho.
?

// E agora, qual a cor do carro?
?

// Mude a cor do carro para verde musgo.
?

// E agora, qual a cor do carro?
?

// Qual a marca e modelo do carro?
?

// Adicione 2 pessoas no carro.
?

// Adicione mais 4 pessoas no carro.
?

// Faça o carro encher.
?

// Tire 4 pessoas do carro.
?

// Adicione 10 pessoas no carro.
?

// Quantas pessoas temos no carro?
?
```
