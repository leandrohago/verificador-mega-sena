# Verificador Mega-sena

Um verificador simples de jogos da mega-sena para quem participa de bolões e precisa verificar vários jogos.

O arquivo consiste em um único **html** com **css** e **javascript** para facilitar a conferência em celulares.

# Configurando

Edite o **array** de objetos **jogos**
```javascript
const jogos = [
	{
		jogador: 'Jogador_1',
		jogos: [
			[05,17,18,30,32,38,43,49,56,60],
			[03,10,15,19,24,27,37,46,48,49],
		]
	},
	{
		jogador: 'Jogador_2',
		jogos: [
			[01,16,23,28,39,44,47,50,55,59],
		]
	},
]
```
Após editado, salve o arquivo e utilize a verificação **online** ou **offline**.

## Online
A verificação **online** faz uma consulta no endereço [https://loteriascaixa-api.herokuapp.com/api/mega-sena/latest](https://loteriascaixa-api.herokuapp.com/api/mega-sena/latest).
Caso retorne algum erro será informado para utilizar a consulta **offline**.

## Offline
Ao utilizar a verificação **offline** é necessário informar as seis dezenas para verificação.