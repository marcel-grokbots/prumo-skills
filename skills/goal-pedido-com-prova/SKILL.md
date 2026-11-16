---
name: goal-pedido-com-prova
description: Ajuda a escrever um pedido /goal que faz a IA trabalhar até a prova de pronto aparecer na tela. Use quando a pessoa quer que uma tarefa longa (organizar pasta, montar planilha, juntar anotações ou listas) termine sem precisar digitar "continua", ou pede ajuda para escrever um /goal no Claude Code ou no app do ChatGPT para computador.
---

# /goal com prova de pronto

O /goal é um comando em que a pessoa escreve uma vez o que precisa ficar pronto e como provar que ficou. A IA trabalha sozinha, rodada após rodada, até essa prova aparecer na tela.

Esta skill ajuda a transformar um pedido vago num /goal bem escrito. Ela não executa o /goal sozinha: entrega o texto pronto para a pessoa conferir e mandar.

## Onde o /goal funciona

- No Claude Code, pelo terminal ou pelo app do Claude para computador.
- No app do ChatGPT para computador.
- Não funciona no chat do navegador, nem no claude.ai nem no chatgpt.com.

Se a pessoa estiver no navegador, avise isso antes de escrever o pedido.

Referências oficiais: https://code.claude.com/docs/en/goal e https://learn.chatgpt.com/docs/reference/slash-commands

## A receita em três partes

Todo /goal precisa ter:

1. O que fazer.
2. Como saber que acabou. Um número ou uma lista que apareça na tela e que a própria IA consiga conferir.
3. O que a IA não pode mexer.

## Como conduzir

1. Pergunte, uma coisa por vez, o que falta das três partes. Não suponha nome de pasta, de arquivo ou de coluna.
2. Transforme "como saber que acabou" numa conta que feche. Exemplos: arquivos antes igual a arquivos depois, PDFs na pasta igual a linhas na planilha, repetidos mais únicos igual ao total.
3. Inclua o que fazer com o caso duvidoso (por exemplo, uma pasta "revisar" ou a palavra "ilegível"), para a IA não chutar.
4. Inclua o que não pode ser apagado, renomeado ou alterado.
5. Devolva o /goal num bloco só, pronto para colar, e lembre a pessoa de rodar primeiro numa cópia da pasta.

## Pedido fraco contra pedido bom

Fraco:

```text
/goal organize minhas notas fiscais
```

Bom:

```text
/goal crie a planilha notas.csv com data, fornecedor e valor de cada PDF da pasta notas. Não apague nem renomeie nenhum arquivo. Se um PDF não der para ler, escreva "ilegível" na linha dele. No fim, me mostre quantos PDFs há na pasta e quantas linhas a planilha tem. Está pronto quando os dois números forem iguais.
```

No fraco, a IA não tem como saber quando acabou. No bom, ela mesma vê se a conta bate.

## Outros modelos para adaptar

Exemplos ilustrativos, ainda não testados. Troque os nomes de pasta e de arquivo pelos da pessoa.

Organizar uma pasta bagunçada:

```text
/goal organize os arquivos da pasta Downloads em subpastas por assunto, como clientes, impostos e viagens. Não apague nenhum arquivo. Se não tiver certeza de onde um arquivo vai, coloque na pasta revisar. Anote cada mudança no arquivo mudancas.csv, com o lugar antigo e o novo. No fim, me mostre quantos arquivos havia antes, quantos há depois e quantos ficaram soltos fora das subpastas. Está pronto quando antes e depois forem iguais e nenhum arquivo estiver solto.
```

Juntar anotações espalhadas num resumo:

```text
/goal leia todos os arquivos da pasta reunioes e crie o arquivo resumo.md com uma seção para cada arquivo, com as decisões e as pendências daquela reunião. Não altere os arquivos originais. Se uma reunião não tiver decisão, escreva "sem decisão" na seção dela. No fim, me mostre quantos arquivos há na pasta e quantas seções o resumo tem. Está pronto quando os dois números forem iguais.
```

Juntar listas de clientes sem repetir ninguém:

```text
/goal junte as planilhas da pasta clientes numa só, chamada clientes-unificado.csv. Considere repetido quem tiver o mesmo e-mail e deixe só uma linha dessa pessoa. Não altere as planilhas originais. No fim, me mostre o total de linhas somando todas as planilhas, quantas repetidas você tirou e quantas ficaram. Está pronto quando as que ficaram mais as repetidas derem o total.
```

## Cuidados para passar à pessoa

1. Na primeira vez, rodar numa cópia da pasta.
2. No ChatGPT, começar com /plan para montar o objetivo e depois mandar o /goal.
3. Para parar antes do fim: no Claude Code, digitar /goal clear. No ChatGPT, usar os botões acima da caixa de texto.
4. Se a IA pedir permissão para alguma ação, ela espera a resposta.
5. "Terminei" é a palavra da IA, não a prova. Conferir por amostra: abrir três itens do resultado e comparar com a origem.

---

Parte da coleção aberta do Prumo (https://prumo.academy). Mais em https://mscreative.systems
