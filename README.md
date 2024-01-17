
Mouse Movement para o player
-

Este código foi criado durante 3 dias e algumas horas, pegando de refêrencia videos, informações na documentação e na internet. Juntei essas informações, quebrei um pouco a cabeça e deu nesse código. Ele é funcional, mas ainda está em fase de teste e algumas poucas coisas não funcionam como deveriam. Se sinta livre para pegar, editar e usar em seu projeto, caso queira.

Ele funciona de maneira simples, aqui vou fazer um resumo, pois dentro do código existem muitas informações. 
* Você transforma seu mouse em um Target, isso pode ser visto pela CollisionShape2D em volta do cursor.

![Captura de tela 2024-01-17 132759](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/3b20fa20-00c0-4bcd-9e9b-091c1afc7e9d)

Com ele você define onde vai atirar, como em muitos jogos rogue-like. Mas o diferencial é que não é a arma que gira para acompanhar seu personagem, mas sim a sprite. 
* Caso o jogador mire o cursor para baixo, a sprite muda para ele de frente. Caso gire o cursor para a diagonal, a sprite do player em diagonal entra.

![Captura de tela 2024-01-17 134159](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/25793309-cbc6-42b1-ab27-14e546d06a88)

Para que o código funcione, você precisa ter esses nodes e childs:

Player:
![Captura de tela 2024-01-17 132311](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/69ea89dd-2586-4c09-b52c-bebc7008dcc8)

Bullet:
![Captura de tela 2024-01-17 132339](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/ef588644-f9f8-4a2f-97b0-785200a130f9)

Cada um carrega uma funcionalidade ajustada e outras ainda em reparo para que funcione como deveria. É um código ainda em evolução.

As sprites do seu personagem precisam ser carregadas dentro do AnimatedSprite2D para trazer a mudança junto ao movimento do cursor. Abaixo está as imagens que você deve seguir para conseguir um resultado igual ou parecido com o meu.

Para funcionar você precisara criar um Node de AnimatedSprite2D e nele criar pastas. Essas pastas devem ser chamadas de "run", começa do zero: "run0" e vai até o "run7". Nessas pastas você vai colocar a animação de movimento do personagem e APENAS uma dele de idle(parado). Em todas você deve seguir essa linha e ter o mesmo número. O meu idle foi o número 4, então em toda pasta ele tem que ser o 4

![Captura de tela 2024-01-17 132709](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/84513cf0-1c30-444c-94c9-f2678ef8a603)
![Captura de tela 2024-01-17 132704](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/c38de0f7-bcbe-4998-88d1-f7275e189f98)
![Captura de tela 2024-01-17 132658](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/f5a10204-112d-4034-aa19-5f412ca58d4f)
![Captura de tela 2024-01-17 132324](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/8cc30677-5839-4ccb-a736-b45d4a7568e6)
![Captura de tela 2024-01-17 132730](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/8006b892-ca0b-4713-964e-7b2e5bd88472)
![Captura de tela 2024-01-17 132725](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/e8e03842-8a3a-409c-9afa-cf3ba44526d6)
![Captura de tela 2024-01-17 132721](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/c562e9bf-bf85-4e1a-9282-984c4524a712)
![Captura de tela 2024-01-17 132716](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/bbac10e4-a556-47a8-be74-f76103c23473)

Com isso, seu código já pode estar pronto para ser usado, assim como o meu.

![Vídeo sem título](https://github.com/KaySDellaCapa/mouse-moviment/assets/140545612/f99d0912-ebad-432a-8943-3148db31163a)

