## 01. Controlando o navegador

Para que serve o arquivo chromedriver utilizado nos testes?  
- Para o Selenium WebDriver conseguir se comunicar com o Google Chrome.  
  Os drivers servem como ponte entre a API do Selenium WebDriver e o navegador instalado no computador.
  
Caso de um erro que o driver nõ é executável : chmod +x chromedriver 

Resumo:
- Existem diversos módulos do Selenium, dentre eles o WebDriver;
- Aprendemos como adicionar o Selenium WebDriver no projeto, como uma dependência do Maven;
- Aprendemos a adicionar o Driver do navegador no nosso projeto;
- Aprendemos a escrever um código de teste que abre uma janela do navegador e navega para uma página, utilizando a API do selenium WebDriver.


## 02. Testando o login

Qual a maneira correta de encontrar um elemento na página pelo seu id?
- Utilizando o método findElement(By.id(“id”)) da classe WebDriver
  Essa é a maneira correta de encontrar um elemento pelo seu id.

Qual a maneira correta de acessar o código fonte da página utilizando a API do Selenium WebDriver?
- Utilizando o método getPageSource() da classe WebDriver
  Essa é a maneira correta de acessar o código-fonte da página.

Qual a maneira correta de acessar a url atual do browser?
- Utilizando o método getCurrentUrl() da classe WebDriver
  Essa é a maneira correta de acessar a url da página atual.
  
Resumo:
- Que é possível recuperar elementos na página utilizando o método *findElement()*;
- Que é possível recuperar o código fonte da página utilizando o método *getPageSource()*;
- Que é possível recuperar o url atual do browser utilizando o método *getCurrentUrl()*;
- Que devemos utilizar o método *sendKeys()* para enviar textos para os inputs da página;
- Que uma das maneiras de submeter um formulário é via método *submit()*.


## 03. Page Objects

Quais as vantagens de se utilizar o padrão Page Object?
- Favorecer a separação de responsabilidades
  Ao utilizar o padrão Page Object favorecemos a separação de responsabilidades entre os códigos de testes e de utilização da API do Selenium WebDriver.

- Melhorar a legibilidade dos códigos de testes
  O padrão Page Object reduz bastante a verbosidade dos códigos de testes, os tornando mais legíveis.
  
Resumo:
- O que é o padrão Page Object;
- As vantagens de se utilizar o padrão Page Object;
- Como implementar o padrão Page Object com classes Java.


## 04. Testes do cadastro de leilão

Qual o tipo de objeto devolvido pelo método findElement()?
- WebElement
  O método findElement devolve um objeto do tipo WebElement, que pode ser atribuído a uma variável.

Quais são as maneiras de submeter um formulário?
- Chamando o método submit() a partir de um input recuperado pelo findElement().
  Essa é uma das maneiras possíveis de submeter um formulário.

- Chamando o método submit() a partir de um formulário recuperado pelo findElement().
  Essa é uma das maneiras possíveis de submeter um formulário.
  
- Chamando o método click() a partir de um botão de submit recuperado pelo findElement(). 
  Essa é uma das maneiras possíveis de submeter um formulário.
  
Resumo:
- Que o método findElement() devolve um objeto do tipo WebElement;
- Que não devemos enviar null pelo método sendKeys() ao testar campos vazios;
- Que um objeto Page Object pode devolver outro Page Object quando ocorre uma navegação entre páginas;
- Que podemos reaproveitar o objeto WebDriver entre diferentes objetos Page Object;
- Que podemos recuperar um elemento na página a partir de outro elemento;
- Que podemos utilizar herança, design patterns, dentre outras práticas para organizar os códigos de testes da aplicação.

## 05. AJAX e boas práticas

Como lidar com requisições AJAX ou códigos JavaScript que podem adiar o carregamento de elementos na página?
- Configurando um Timeout pelo metodo webDriver.manage().
  É possível configurar diferentes tipos de Timeout pelo Selenium WebDriver.

Quais das seguintes alternativas são recomendações citadas no Guideline de boas práticas do Selenium WebDriver?
- Utilizar Page Objects
  Essa é uma das boas práticas citadas no Guideline.
- Evitar compartilhar estado
  Essa é uma das boas práticas citadas no Guideline.

Resumo: 
- Que alguns testes podem falhar quando a aplicação utilizar códigos JavaScript, como por exemplo em chamadas AJAX;
- Que é possível configurar diferentes Timeouts na API do WebDriver;
- As boas práticas recomendadas no [Guideline do Selenium WebDriver](https://www.selenium.dev/documentation/en/guidelines_and_recommendations/)





