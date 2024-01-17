
Mouse Movement para o player
-

Este código foi criado durante 3 dias e algumas horas, pegando de refêrencia videos, informações na documentação e na internet. Juntei essas informações, quebrei um pouco a cabeça e deu nesse código. Ele é funcional, mas ainda está em fase de teste e algumas poucas coisas não funcionam como deveriam. Se sinta livre para pegar, editar e usar em seu projeto, caso queira.

Ele funciona de maneira simples, aqui vou fazer um resumo, pois dentro do código existem muitas informações. 
* Você transforma seu mouse em um Target, isso pode ser visto pela CollisionShape2D em volta do cursor.


![Captura de tela 2024-01-17 134159](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/eb29faad-124f-4070-9580-f3c7d2b3a0b6)

Com ele você define onde vai atirar, como em muitos jogos rogue-like. Mas o diferencial é que não é a arma que gira para acompanhar seu personagem, mas sim a sprite. 
* Caso o jogador mire o cursor para baixo, a sprite muda para ele de frente. Caso gire o cursor para a diagonal, a sprite do player em diagonal entra.

IMAGEM EM diagonal

Para que o código funcione, você precisa ter esses nodes e childs:

IMAGEM do node player

Imagem do node bullet

Cada um carrega uma funcionalidade ajustada e outras ainda em reparo para que funcione como deveria. É um código ainda em evolução.

As sprites do seu personagem precisam ser carregadas dentro do AnimatedSprite2D para trazer a mudança junto ao movimento do cursor. Abaixo está as imagens que você deve seguir para conseguir um resultado igual ou parecido com o meu.

Para funcionar você precisara criar um Node de AnimatedSprite2D e nele criar pastas. Essas pastas devem ser chamadas de "run", começa do zero: "run0" e vai até o "run7". Nessas pastas você vai colocar a animação de movimento do personagem e APENAS uma dele de idle(parado). Em todas você deve seguir essa linha e ter o mesmo número. O meu idle foi o número 4, então em toda pasta ele tem que ser o 4

Imagens das pastas

Com isso, seu código já pode estar pronto para ser usado, assim como o meu.

Video
