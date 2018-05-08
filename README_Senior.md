# Desafio - Desenvolvedor iOS 

Nós do time de mobile do Grupo Zap VivaReal gostamos de jogar videogames. Gostaríamos de saber quais são os **Top Games no Twitch**. 🤓🎮

O objetivo do teste é implementar um app onde podemos ver os jogos com mais visualizações no Twitch. O app deve mostrar uma lista de jogos e ser possível navegar para os detalhes de cada jogo. Além disso, tanto na lista quanto na tela de detalhes, deve ser possível favoritar o jogo. Os jogos favoritados devem ser persistidos no device para que possam ser acessados offline e serem mostrados em uma aba própria.

## API

Para desenvolver o app você vai precisar usar o endpoint de Top Games do Twitch. Mais informações: https://dev.twitch.tv/docs/v5/reference/games/.

## Interface

A interface do app é dividida em 3 partes e deve ser desenvolvida conforme os pontos abaixo.

### Home - Top Games

* Listagem dos jogos ordenados por visualização.
* Botão para favoritar jogos nas células.
* Barra de busca para filtrar lista de jogos por nome.
* Pull-to-refresh para atualizar a lista.
* Paginação na lista: Carregar 20 jogos por vez, baixando a próxima página ao chegar no fim da lista.

### Detalhes do jogo

* Botão de favorito.
* Foto em tamanho maior, nome e número de visualizações do jogo.

### Favoritos

* Listagem dos jogos favoritados pelo usuário.
* Favoritos devem ser persistidos para serem acessados offline.
* Interface de lista vazia caso o usuário não tenha favoritos.

### Wireframe

Abaixo temos os wireframes das telas do app.

Se você pensou em alguma *killer feature* que acabamos deixando de fora do nosso backlog, sinta-se a vontade para implementar. **Use sua imaginação!** 🤓

| ![Page1](images/Page1.png)  | ![Page2](images/Page2.png) | ![Page3](images/Page3.png) |
|:---:|:---:|:---:|
| Lista de Top Games | Jogos Favoritos | Detalhes do Jogo |

## Requisitos Essenciais

* Usar Swift 4.
* Interface desenvolvida no **Storyboard**, utilizando Auto Layout.
* Usar UICollectionView com no minimo **2 colunas** para representar a lista dos jogos e favoritos.
* App Universal: Você deve desenvolver uma interface que se adapte bem em telas maiores.
* CoreData: Favoritos devem ser salvos no **CoreData** para que os usuários consigam acessar offline.
* Tratamento de falha de conexão: Avise o usuário quando o download dos jogos falhar por falta de conexão.
* Today Widget: Um Widget onde podemos visualizar rapidamente os 3 jogos mais populares do Twitch. 
* Drag and Drop: Implemente uma interação com Drag and Drop onde podemos selecionar um jogo da lista principal e arrastar para a lista de favoritos, favoritando o jogo.
* Testes unitários.
* Integração com Fastlane com uma lane para rodar os testes unitários.
* **O teste não pode apresentar crashes.**

**A falta de algum requisito essencial é eliminatória.**

## Bônus

* Imagina que legal poder acessar os jogos através do iMessage para compartilhar com os amigos. 😜

## Observações

* Você pode utilizar bibliotecas de terceiros e gerenciadores de dependências (CocoaPods, Carthage, etc) como preferir.
* Foque o desenvolvimento nos requisitos essenciais. O bônus vai diferenciar você dos outros candidatos, mas **os requisitos essenciais são mais importantes**.
