---
title: "Blog Craveiro"
description: "Como eu construi o meu blog."
permalink: /blog-craveiro
category: "Desenvolvimento de sites"
image:
  path: /2019/02/print-craveiro.png
  alt: "Uma printscreen da tela inicial do blog Craveiro."
---

O meu objetivo era fazer um blog aonde além de ser leve e customizável, não fosse necessário gastar um centavo em hospedagem. Pesquisando pela internet, encontrei um conceito chamado **Jamstack**. 

Pesquisando sobre isso, decidi fazer meu blog em Jekyll. Com ele é possível fazer um blog absurdamente leve (a página deste blog carrega em 0.1ms e pesa menos de 15kb(!) ), totalmente customizável e é possível hospedar no próprio Github Pages, ou em plataformas como Netlify (aonde este blog está hospedado).

Este blog está em constante evolução, mas estas tecnologias já estão disponíveis:

## Imagens responsivas

Através do plugin Jekyll Picture Tag, é possível inserir uma imagem e ele automaticamente gerar versões nos mais diversos tamanhos e formatos para se adaptar de acordo com o dispositivo do usuário. Isso torna o blog ainda mais leve.

## Tipos de postagens customizadas

Além da área tradicional de posts, há uma área separada para o portfolio e uma de poemas, tudo diretamente no mesmo blog.

## SEO

O SEO deste blog suporta o Open Graph, Twitter Cards e Schema.org, para o melhor aproveitamento das redes sociais e desempenho nos mecanismos de busca. Você pode dar uma olhada no código [aqui](https://github.com/raulcraveiro/craveiro/blob/master/_includes/head.html).

## Tecnologias utilizadas

- **Jekyll** para o desenvolvimento do blog;
- **Github** como repositório de código;
- **Netlify** para o deploy;

Todo o código do blog é open-source e encontra-se disponível no [Github](https://github.com/raulcraveiro/craveiro/).