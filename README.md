# Docker

## Introdução

Imagine que seja necessário executar um sistema que depende de diversas aplicações, todas elas consumindo recursos e armazenamento da sua máquina e rodando nas mesmas portas, rapidamente é perceptivel que isso não seria viável.
Uma alternativa seria rodar cada aplicação em uma máquina, mas imagine um sistema com várias aplicações, seria necessário muito dinheiro para investir em todos esses recursos.

Logo, podemos pensar na ideia da utilização de máquinas virtuais no entanto existe uma quantidade consideravel de recursos computacionais necessários para isso, pois cada VM simula um sistema operacional completo, logo uma máquina teria que ter a capacidade de processar todas essas virtualizações.

Por fim, a idéia mais viável seria a utilização de containers, eles permitem que seja virtualizado uma porção enxuta do sistema operacional com as dependências necessárias para a execução.

## Docker Hub

O docker hub funciona como um grande repositório de **imagens**, por meio dele podemos executar uma imagem:

```bash
docker run hello-world
```

Esse código irá verificar se a imagem 'hello-world' já existe localmente em sua máquina, caso não encontre ele fará o download dela e irá executá-la exibindo uma mensagem no terminal indicando que o docker está funcionando.

Além disso podemos baixar as imagens para a nossa máquina, então utilizando do mesmo exemplo de cima:

```bash
docker pull hello-world
```

E agora a imagem hello-world será baixada e vai estar disponivel em sua maquina, no entanto, caso você digite ```docker run hello-world``` o container não será inicializado e trataremos do porque disso mais abaixo.
