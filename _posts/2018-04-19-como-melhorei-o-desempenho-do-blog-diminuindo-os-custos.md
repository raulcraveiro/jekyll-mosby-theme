---
title: "Como melhorei o desempenho do blog diminuindo os custos"
description: "Zerei os custos de servidor do blog e ainda aumentei absurdamente o desempenho."
permalink: /melhorei-desempenho-diminuindo-custos
category: tecnologia
image:
  path: /2018/04/dinheiro.jpg
  alt: "Uma mão segurando uma carteira com duas notas de 100 dólares e ao fundo um notebook desfocado."
---

O meu plano de hospedagem do blog estava próximo de expirar, e como eu ainda estou na estatística do desemprego, tive que pensar em uma alternativa para manter o meu blog sem gastar dinheiro.

Anteriormente, o meu blog era publicado pelo Wordpress no servidor da [Hostgator](https://www.hostgator.com.br/28343.html). Nunca tive nenhum problema com a Hostgator, muito pelo contrário, eu recomendo muito, mas eu nunca gostei da plataforma Wordpress. Aí aproveitei a oportunidade para dar uma aventurada.

## Mudança de plataforma

Eu sabia da existência dos geradores de sites estáticos, mas nunca tinha levado tão a sério. Foi aí que resolvi dar uma pesquisada no Jekyll.

Procurando por temas, encontrei um port do tema principal do Ghost para Jekyll, chamado [Jasper2](https://github.com/jekyller/jasper2). Fiz algumas alterações no tema, removi alguns códigos desnecessários, adicionei os links das minhas redes sociais, entre outras coisas. Um dos problemas estava resolvido.

## Hospedagem

Depois de decidir qual gerador e tema utilizar, chegou a hora de escolher aonde hospedar o código. A principal forma é através de um repositório de códigos, e as principais plataformas são: Github, Bitbucket e Gitlab. Decidi pelo Github, por ser a principal plataforma e ter compatibilidade com o Netlify CMS (já vou explicar o que é).

## Deploy

De uma maneira leiga, dar deploy em um código é "colocar ele pra funcionar", fazendo gerar os arquivos finais, que serão disponibilizados para o público que acessar o site. Utilizando o Github, é possível fazer isso dentro da própria plataforma utilizando o Github Pages, que tem suporte nativo ao Jekyll. Porém, decidi utilizar uma outra plataforma chamada Netlify, que oferece algumas outras ferramentas que me ajudam no desempenho do blog.

Pelo Netlify, consigo compactar todo o código, as imagens e ainda disponibilizar SSL no site sem pagar nada.

## Criando conteúdo

Com tudo isso decidido, faltava resolver como eu criaria os novos posts. Teoricamente, utilizando um gerador de site estático, você cria os arquivos de posts manualmente, criando um arquivo markdown, aplicando o Front Matter e depois fazendo o merge (algo semelhante à fazer upload) para o Github.

Mas pesquisando, descobri que existem alguns gerenciadores de conteúdo que facilitam na hora da criação dos posts. Cheguei a testar dois serviços: [Forestry](https://forestry.io/) e [NetlifyCMS](https://netlifycms.org/), mas por já utilizar o serviço do Netlify, optei pela segunda opção.

A configuração do CMS é bem simples: basta criar uma pasta chamada admin, inserir um arquivo index.html com um código padrão que servirá para realizar o login, e um arquivo config.yml aonde é possível adaptar a plataforma para a sua utilização, e definir o Front Matter dos seus posts.

A parte mais interessante desse CMS, é que ao salvar o rascunho, ele realiza um deploy em um branch separado, não tendo o risco de perder o seu rascunho, e ainda é possível ter um preview de como o seu post ficará no blog.

## Conclusão

Foram alguns (vários) dias mexendo em códigos, realizando diversos testes, quebrando a cabeça e tendo que aprender muitas coisas novas. Mas além de diminuir o meu gasto de 160 reais anuais em servidor pra 0 (!) reais, eu ainda aumentei absurdamente o desempenho, já que um gerador de código estático é feito basicamente de arquivos HTML, CSS e JS, sem ter a necessidade de um banco de dados.
