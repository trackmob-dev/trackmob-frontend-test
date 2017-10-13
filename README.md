
# **Trackmob - Teste para Frontend - Página de Doação**

## Sobre este teste

A Trackmob é uma empresa focada em desenvolver produtos que auxiliam ONGs a gerenciam suas tarefas de captação de recursos, possibilitando uma experiência de doação incrível para seus doadores.

Com este objetivo, um de nossos produtos consiste numa página de doação personalizada, para que pessoas interessadas em ajudar a ONG se inscrevam e comecem a doar.
Este teste consiste em implementar uma versão simples de um de nossos modelos de página de doação.

## A Tarefa

Faça um fork deste repositório e nos envie o link com sua implementação.

Você será responsável por implementar a página abaixo (você pode baixar o PSD através deste [link](https://drive.google.com/file/d/0B6UrrFcFJAjXRHdNZUJTYnJsd2s/view?usp=sharing))

![Layout da página](https://i.imgur.com/9tcPGHS.png)

Você deve executar os seguintes pontos:

- Finalizar a página seguindo as guias e o exemplo no arquivo PSD (use o GIMP caso não possua o Photoshop)
- Implementar a validação de e-mail, exibindo o erro como no exemplo.
- O selectbox de frequência deve ter as seguintes opções: "Única", "Mensal", "Semestral", "Anual"
- O valor inserido e a frequência devem mudar o valor ao lado do botão de confirmação (R$ 35 mensais no exemplo)
- Todos os campos são necessário, mostre com um erro os campos esquecidos ao submeter o formulário
- Se todo os campos estiverem preenchidos e validados, você deve enviar os dados para a API REST

## API REST

Você irá executar um POST na sequinte URL:
`https://trackmob-frontend-test.firebaseio.com/RdMa77REkLXsh9ec0WcWNbff1dw2/<github_username>/donors.json`

Troque **<github_username>** pelo seu login no github

Envie os dados no seguinte formato JSON:
```javascript
{
	"frequency": "Mensal",
	"value": "30.00",
	"first_name": "João",
	"last_name": "da Silva",
	"complete_name": "João da Silva",
	"email": "joao@silva.com.br",
	"document": "12345678909",
	"card_number": "4111111111111111",
	"cvv": "123",
	"validity": "01/2020",
	"accept_contact": true
}
```

## Tarefas Bônus

- Use React
- Implemente máscaras e validação para todos os campos
- Implemente validação no evento de blur
- Faça o layout responsivo
- Torne o layout acessível
- Publique sua aplicação e nos mande o link para acesso
- Adicione uma boa cobertura de testes no seu código

## Critérios de avaliação

- Código limpo, bem estruturado e bem comentado
- Fidelidade ao layout
- Bom uso de git
- Qualidade e quantidade de bônus implementados
- Experiência do usuário
