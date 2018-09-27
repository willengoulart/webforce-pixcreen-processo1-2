## Atividade de Front

Para a atividade de seleção, você deve criar duas páginas web como descritas abaixo.
**As duas páginas devem ser responsivas.**

### Página 1: Lista de Influencers

Essas informações devem ser acessadas por requisição AJAX via Axios.
Para isso, basta fazer uma requisição GET para a URL: https://pixcreen.com/followers/open/topic-channels/393/json/

Para fazer a chamada Ajax, e popular os dados na página que criou, você deve usar VueJS.

Use o Bootstrap como base para o seu CSS e faça alterações no layout usando seus conhecimentos em CSS.
Fique à vontade para criar o seu próprio layout.
Quando mais complexo e bonito, melhor você se sairá. Você pode usar o Card ou o List Group do Bootstrap.

#### Sobre o retorno do Serviço
Os dados dos influencers estão no atributo channels. Basta iterá-lo para listar os influencers no assunto.
Dentro de cada channel, você encontrará os seguintes atributos:
- avatar: link para a foto de perfil do Influencer
- howManyPosts: Quantos posts aquele Influencer já tem
- influencer_bio: descrição sobre o Influencer
- influencer_name: Nome do Influencer
- master: true se ele é o Master-Influencer do assunto, aquele que tem mais seguidores. False caso não seja.

Você deve OBRIGATORIAMENTE apresentar todos esses dados na tela e ignorar os outros.


### Página 2: Canal do Influencer

Para acessar as informações do Influencer, você deve fazer uma requisição GET para a seguinte URL: 
https://pixcreen.com/open/channel/[channel_id]/json/ onde [channel_id] é o valor channel_id que você obtém usando os dados da atividade anterior.

#### Sobre o retorno do serviço
Os dados do influencers estão no atributo channel.
Dentro de channel, você encontrará os seguintes atributos:
- avatar: link para a foto de perfil do Influencer
- howManyPosts: Quantos posts aquele Influencer já tem
- influencer_bio: descrição sobre o Influencer
- influencer_name: Nome do Influencer
- master: true se ele é o Master-Influencer do assunto, aquele que tem mais seguidores. False caso não seja.

Para mostrar os posts do usuário, você deve iterar o atributo posts.
Dentro de posts você encontrará as seguintes informações:
- body: Texto do Post
- claps: Número de Claps(Likes) que o post recebeu.
- friendlyLink: Link direto para o post
- postPicture: Se não estiver vazio é a imagem do Post.
- videoLink: Se não estiver vazio, o post tem um video do Youtube.
O código é o código do vídeo no Youtube. Use o embeb do Youtube para mostrar o vídeo na página
- pubDate: Data e hora de publicação do post
- title: Título do Post

Novamente, todas as informações acima deve estar disponíveis na sua página.


### Links Úteis
https://getbootstrap.com/docs/4.1/getting-started/introduction/

https://vuejs.org

https://pixcreen.com/canal/astrologia/bruna-said?src=pixcreen (Canal real de uma Influencer. Você pode utilizar os ícones dessa página ou utilizar outros)


## Atividade de Back

Para a atividade de seleção você deve fazer um arquivo PHP que funcione da seguinte forma:

```
/index.php?email=[EMAIL]&cpf=[CPF]
```

e imprima na tela se o E-mail e o CPF são válidos.

Exemplo:

```
/index.php?email=wgoulart@pixcreen.com&cpf=00000000000
```

Mostra na tela:

```
Seu E-mail wgoulart@pixcreen.com é válido

Seu CPF 000.000.000-00 é inválido.
```

**OBS:** Note que você deverá receber o CPF sem pontos e vírgulas e deverá imprimí-lo com pontos e traço

**OBS2:** Nessa atividade você precisará instalar um servidor Web e o PHP. Para isso, sugerimos a instalação do WampServer

**OBS3:** Você pode simplificar a validação do E-mail testando se ele tem um "@" e ".com".

### Links Úteis
https://howtoubuntu.org/how-to-install-lamp-on-ubuntu

http://www.wampserver.com/en/

http://php.net/manual/en/function.preg-match.php

## Considerações finais

- As atividades exigem mais do que você sabe e nossa intenção não é que você finalize, mas o quanto você conseguiu avançar na tarefa proposta.
- Use a internet a seu favor. Você é livre pra buscar aquilo que tem dúvida e não sabe. Google e StackOverflow são seus amigos.
- Envie seu código mesmo que não esteja completamente funcional. Comente suas dificuldades no código. Vamos levar em conta todo o seu esforço.
- A atividade é aberta à sua interpretação e melhoria. Se algo não ficou claro, você pode fazer como entendeu e comentar no seu código, assim como utilizar outras ferramentas mais complexas.
- Entregue seu código em um repositório público do GitHub e nos mande o link. Faça commits pequenos mostrando o quanto você caminhou.
- Essas duas páginas já estão disponíveis no Pixcreen. Você pode se cadastrar e usá-las como inspiração.
