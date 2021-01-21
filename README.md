# Ruptiva - Code Challenge Front-end

## Introdução

Este é um desafio utilizado como teste de desenvolvimento Front-end pela Ruptiva.

Na empresa, desenvolvemos diversos projetos de aplicativos e sistemas web, portanto, algumas ferramentas são necessárias para manter o desenvolvimento sadio do projeto desde sua fase de planejamento até sua fase de implementação em produção.

Das ferramentas que costumamos utilizar:

- Git
- HTML
- CSS/SASS
- Typescript
- RESTful APIs
- React/React Native

O pessoal do back-end utiliza Ruby on Rails e PostgreSQL.

Neste teste serão avaliados:

- Funcionalidade - todas especificações atendidas
- Código - o código limpo utilizando boas práticas de desenvolvimento e [estilo](https://github.com/ruptiva/frontend-styleguide)
- Commits - realização constante de commits com descrições significativas
- Testes
 

## Requisitos Técnicos

- O projeto deve ser escrito em Typescript
- Os componentes devem ser, sempre que possível, `stateless`
- Arquivos de renderização não podem conter métodos relacionados a busca, envio ou tratamento de dados

**Pontos extras:**
- Hooks
- JSDoc
- Programação funcional

## Requisitos Funcionais

Crie um [snack](https://snack.expo.io/) com uma única tela, contendo um formulário que solicita um documento do usuário (CPF ou CNPJ) e seu nome (pessoa física) ou razão social (pessoa jurídica). Ambos os campos são obrigatórios, mas o botão de envio do formulário não pode ficar desativado em nenhum momento.

Os campos devem apresentar erros de validação, tanto no formato do documento, quanto a ausência do nome/razão social. No campo de documento, uma máscara deverá ser exibida de acordo com o tipo do documento.

Inicie um novo projeto no Firebase, e envie os dados para o [Firestore](https://firebase.google.com/docs/firestore/?hl=pt-br), seguindo a seguinte estrutura:

```js
{
  name: 'Lorem ipsum',
  document: '12345678900', // deve conter apenas números
  type: 'individual' // ou 'business' no caso de pessoa jurídica/CNPJ
}
```

Ao efetuar o envio, os campos do formulário devem ser desabilitados e o botão deve ser substituído por um spinner, com a mensagem `Enviando`. Quando a resposta da requisição for recebida pelo seu snack, o formulário deve voltar para seu estado inicial.

Abaixo do formulário, adicione o título 'Usuários'. Exiba uma lista dos usuários que você cadastrou, e permita que a lista seja atualizada quando o conteúdo for 'puxado' para baixo. Cada item da lista deve possuir o nome do usuário e seu documento com a máscara correta. Diferencie os tipos de usuário com as cores laranja (`#ff6a00`) e azul (`#00b2ff`). Adicione também a opção de excluir um registro, solicitando a confirmação do usuário.

#### Testes

- Testes de snapshot
- O que julgar necessário

## Entrega

- Criar um repositório público ou privado para avaliação do time Ruptiva
- Criar um `README.md` no repositório com uma breve descrição do processo de desenvolvimento, incluindo problemas/dificuldades encontradas e um link para o snack.
- A partir do momento que você recebeu este teste, tem 5 dias para concluí-lo. Caso não consiga entregar no prazo, entre em contato para justificar o motivo.
- O contato deve ser feito pelo do e-mail cleimar@ruptiva.com
