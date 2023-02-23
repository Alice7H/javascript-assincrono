## Fundamentos de Javascript Assíncrono

Ministrado por Stephany Nusch

## Conteúdo

`Assíncrono` é o que não ocorre ou não se efetiva ao mesmo tempo.

`Promise` é um objeto de processamento assíncrono de um resultado/valor desconhecido que pode ser resolvido ou rejeitado.

Uma promise possui 3 estados:

- Pending: estado inicial, nem cumprido nem rejeitado.
- Fulfilled: significa que a operação foi concluída com sucesso.
- Rejected: significa que a operação falhou.

Estrutura da promise:

```javascript
  const myPromise = new Promise(function(resolve, reject) => {
    setTimeout(()=> { resolve(console.log('Resolvida')); }, 2000);
  });
```

`Async/await` são palavras chaves para definir funções assíncronas.

`APIs` significa Application Programming Interface, é uma forma de intermediar os resultados do back-end com o que é apresentado no front-end. Acessados por meio de URLs.

`JSON` significa Javascript Object Notation e é um formato comum dados usados como retorno das APIs.

`Fetch` é um mecanismo que permite consumir APIs pois fornece uma interface Javascript para acessar e manipular partes do pipeline HTTP (pedidos e respostas) de forma assíncrona.

O fetch faz com que você utilize os métodos `json()` e o `stringify()`.

O método `Response.json()` pega um fluxo Response e o lê até a conclusão. Ele retorna uma promessa que resolve com o resultado da análise do corpo do texto como JSON.

O método estático `JSON.stringify()` converte um valor JavaScript em uma string JSON.

## Atividade:

Criar uma página que carrega fotos aleatórias de gatinhos sempre que clicamos em um botão.

- Utilize a API ~~`https://thatcopy.pw/catapi/rest`~~ substituído por `https://api.thecatapi.com/v1/images/search` para fazer as chamadas com o método fetch();

- Utilize seus conhecimentos na manipulação do DOM para criar a imagem e ativar o evento de clique do botão!

## Materiais de Apoio:

- [Slides - Assincronicidade](https://academiapme-my.sharepoint.com/:p:/g/personal/renato_dio_me/ETPRaviVEUFKuIGGZaGgGgMB5Ah7-Wj4qcIQNpOPsz3_FQ?rtime=gfiGZcoV20g)

- [Slides - Consumindo APIs](https://academiapme-my.sharepoint.com/:p:/g/personal/renato_dio_me/EWXS4O_ioCxFmrZtZuTXYRkB5riV-VGMSfdUKmUUjEhtZA?e=nvqFhd)

- [Documentação - The Cat API](https://developers.thecatapi.com/view-account/ylX4blBYT9FaoVd6OhvR?report=bOoHBz-8t)
