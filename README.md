# Simulador de Loteria
Este projeto é um simulador da *megassena*, onde o usuário digita seis números.
E sorteamos aleatóriamente outros seis números e comparamos para verificar, quantos números
você acertou.

**Não é um simulador oficial**

## Técnologias Utilizadas

1. **HTML** : HTML é uma linguagem de marcação utilizada na construção de páginas na Web.

2. **CSS** : CSS é um mecanismo para adicionar estilo (cores, fontes, espaçamento, etc.) a um documento web.

3. **JS** : javaScript é uma linguagem de programação baseada em scripts e padronizada pela ECMA International (associação especializada na padronização de sistemas de informação).

4. ~~**Jquery**~~ : Não foi utilizado.

## Função Principal

### Funções principais

Aqui sera apresentado as duas funções principais do código do site.
### Sorteio de número

Nessa função os números são sorteados aleatóriamente

```
function sortearNumeros() {
numSort = [];
let sort;
for (var i = 0; i < 6; i++) {
do {
sort = Math.ceil(Math.random() * 60);
sort = (sort == 0) ? 1 : sort;
}while(numSort.includes(sort));
numSort.push(sort);
}
```

### Lendo os números digitados
Lê as entradas de números digitados pelo usúario
```
function addToList(num, pos) {
if (num.length == 2) {
if (numEsco.includes(num)) {
alert("Numero Escolhido Anteriormente!! Digite outro numero!")
}else if(parseInt(num) > 60){
alert("O numero digitado não pode ser maior que 60");
 }else{
numEsco[pos -1] = num;
}
```
## Como rodar o código

> Simplesmente abra baixe o código e abra o arquivo **_index.html_** no seu navegador.
## Exemplo de Tabela
|Exemplo | Valor de exemplo |

## Exemplo de imagens
 Tela 1: Tela de abertura.

![tela 1](/imagens/atl.png)

Tela 2: 6 números digitados, nenhum sorteado.

![tela 2](/imagens/at2.png)



### Refêrencias

* Html: [wikipidia](https://pt.wikipedia.org/wiki/HTML)
* CSS:  [wikipidia](https://pt.wikipedia.org/wiki/CSS)
* JS: [wikipidia](https://pt.wikipedia.org/wiki/JavaScript)
