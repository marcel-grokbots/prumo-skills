---
name: peca-critica-nao-aplauso
description: Examina uma decisão procurando o que pode dar errado, sem elogio e sem dar a resposta pronta. Use quando a pessoa mostra um plano ou uma decisão (contratar, lançar, cobrar, mudar de preço) e quer crítica honesta, ou quando desconfia que a IA só concorda com ela.
---

# Peça crítica, não aplauso

Quando alguém pede à IA para achar o que é bom num plano, ela acha. Isso parece ajuda, mas deixa a pessoa sem ninguém que a contradiga. Esta skill inverte o pedido: procura as causas mais prováveis de a decisão dar errado, cada uma ligada ao que a pessoa escreveu, com um sinal para ver cedo e um teste barato.

Prompt ainda não testado com o público. Trate como versão inicial.

## Antes de começar

1. Peça a decisão em 1 a 3 frases, os dados que a pessoa tem (só números e fatos) e o que está em jogo (dinheiro, tempo, relação com cliente).
2. Peça que ela não diga o que acha no primeiro pedido. Se ela já disse, ignore essa opinião na crítica e avise numa linha.
3. Se faltar informação, liste o que falta em vez de supor.
4. Lembre que dados de clientes ou de terceiros que ela não pode compartilhar não devem ser colados.

## O que entregar

1. Imagine que passaram 6 meses e a decisão deu errado. Escreva as 4 causas mais prováveis, da mais para a menos provável, cada uma em uma frase e ligada a algo que a pessoa escreveu.
2. Para cada causa, um sinal que ela veria cedo e uma ação barata para testar.
3. A pergunta que um cliente cético faria.
4. O que o texto assume sem prova, com o rótulo "suposição".
5. Em uma frase, o que ela precisaria saber para mudar de ideia a favor da decisão.

## Regras

- Não elogie a decisão nem escreva "boa ideia" ou "ótimo plano".
- Não invente números, concorrentes nem estatísticas. Se faltar um dado, escreva "dado que falta: ...".
- Não diga o que a pessoa deve fazer no fim, só o que checar.
- Se a pessoa insistir e você mudar de posição, diga qual fato novo, do que ela escreveu, mudou a sua posição. Se não houver fato novo, diga isso e mantenha a crítica.

## Limites para dizer à pessoa

- A IA continua sendo uma só. Pedir "responda como um investidor cético" muda o tom, não cria uma segunda opinião independente. Use a lista para perguntar a pessoas de verdade.
- Crítica não é veredito. A IA pode exagerar um risco ou deixar de ver um real. Quem decide é a pessoa.
- A IA só conhece o que foi escrito. Sem números, a lista fala de forma geral e marca o que falta.

## Prompt para colar em qualquer chat

Para quem não usa agente, o mesmo pedido funciona colado no ChatGPT, no Claude ou no Gemini:

```text
Quero que você procure o que pode dar errado nesta decisão. Não quero que me anime e ainda não vou dizer o que eu acho.

A decisão (só o que está em jogo, sem a minha opinião): [A DECISÃO, EM 1 A 3 FRASES]
Dados que eu tenho (só números e fatos, sem interpretação): [DADOS]
O que está em jogo: [DINHEIRO, TEMPO, RELAÇÃO COM CLIENTE ETC.]

Faça assim:
1. Imagine que passaram 6 meses e a decisão deu errado. Escreva as 4 causas mais prováveis, da mais para a menos provável, cada uma em uma frase e ligada a algo que eu escrevi acima.
2. Para cada causa, diga um sinal que eu veria cedo e uma ação barata para testar.
3. Escreva a pergunta que um cliente cético me faria.
4. Liste o que o texto assume sem prova, com o rótulo "suposição".
5. Diga em uma frase o que eu precisaria saber para mudar de ideia a favor da decisão.

Regras: não elogie a decisão nem escreva "boa ideia" ou "ótimo plano". Não invente números, concorrentes nem estatísticas: se faltar um dado, escreva "dado que falta: ...". Não diga o que eu devo fazer no fim, só o que checar. Se meu texto não tiver informação suficiente, liste o que falta em vez de supor. Se eu tiver colado uma opinião minha, ignore essa opinião na crítica e me avise numa linha.
```

## Exemplo de resultado (ilustrativo, dados inventados)

> Decisão: subir a mensalidade de R$ 200 para R$ 280 em janeiro. Dados: 12 clientes hoje, o serviço não mudou neste semestre, 2 clientes pediram desconto nos últimos 30 dias.
> Causa 1: clientes antigos saem porque não viram nenhuma melhora (o serviço não mudou). Sinal cedo: quantos respondem "vou pensar" na primeira semana. Teste barato: avisar 5 clientes antes, com o preço novo.
> Suposição: que os 12 clientes aceitam o mesmo aumento.
> Dado que falta: quantos desses 12 já pagam pontualmente e há quanto tempo.

---

Parte da coleção aberta do Prumo (https://prumo.academy). Mais em https://mscreative.systems
