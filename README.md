# Chibi
O Chibi é uma cafeteria/padaria e-commerce. Um projeto full-stack feito por alunos da escola germinare como trabalho da matéria de DAD.


## Tecnologias
* Banco de Dados: MongoDB
* Back-end:
    - Linguagem Java
    - Maven
    - API Spring Boot

* Front-end
    - Node.js
    - React

## Build & Run

### Rodar API
* Certifique-se de ter instalado:
    1. IntelliJ
    2. OpenJDK-21
    3. Maven

#### Passos
1. Clonar o repositório remoto da api spring
```sh
git clone https://github.com/Chibi-E-Commerce/BackEnd.git
```
* OBS: Não coloque em pastas do OneDrive, ele buga tudo.
2. Abra o projeto clonado no IntelliJ
3. Após esperar a IDE indexar o projeto
    1. Clique no botão M na barra lateral
    2. Expanda o projeto
    3. Vai em lifecycle e rode `clean` e `install`

4. Aperte no botão de rodar a API

### Rodar o Front-end
* Certifique-se de ter instalado:
    1. Node.js (npm / npx)

1. Clonar o repositório remoto do Front-end
```sh
git https://github.com/Chibi-E-Commerce/FrontEnd.git
```
2. Entre no repositório
```
cd ./FrontEnd/
```
3. Instale as dependências com o npm
```
npm install
```
4. Inicie o projeto
```
npm start
```

## Conteúdos Front-end
### Tela de Shopping
Essa tela é onde o usuário deve procurar por produtos a comprar.

#### Filtros
Tipos de Filtro:
* Preço no mínimo R$ ...
* Preço no máximo R$ ...
* Marca ...
* Categorias ...
* Em desconto

#### Categorias
Cada produto terá um `array` de categorias. As categorias que o chibi suportam são: 
- Bebidas
- Doce
- Salgado
- Quente
- Gelado

Documentação / Especificações do Chibi

#### Cálculo do desconto
Pega-se o preço do banco e aplica a seguinte fórmula:
```
                       100 - desconto
com_desconto = preco * --------------
                            100
```