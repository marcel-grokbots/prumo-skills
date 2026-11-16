# prumo-skills

Skills abertas do Prumo para quem já trabalha com agentes de IA. Cada skill é uma pasta com um arquivo `SKILL.md`, no padrão aberto Agent Skills (https://agentskills.io), e funciona no Claude Code, no Codex e no Cursor.

Estas skills saem das fichas da Biblioteca do Prumo, o curso de IA para o dia a dia do Prumo.Academy. Esta é a parte aberta. O curso completo fica para quem é aluno.

## O que tem aqui

| Skill | Para que serve |
|---|---|
| [`goal-pedido-com-prova`](skills/goal-pedido-com-prova/SKILL.md) | Escrever um pedido /goal com as três partes (o que fazer, como saber que acabou, o que não mexer), para a IA trabalhar até a prova aparecer na tela. O /goal funciona no Claude Code (terminal ou app do Claude para computador) e no app do ChatGPT para computador. Não funciona no chat do navegador. |
| [`peca-critica-nao-aplauso`](skills/peca-critica-nao-aplauso/SKILL.md) | Examinar uma decisão procurando o que pode dar errado, com sinal cedo e teste barato para cada risco, sem elogio e sem resposta pronta. |

### Prompt Chain (repositório próprio)

A terceira skill da coleção é a Prompt Chain, que já tem repositório próprio: https://github.com/1marcelserrano/prompt-chain (licença MIT, versão v2.3.0). Ela divide um trabalho grande em pedidos para conversas novas, em sequência (cada etapa gera o pedido da próxima) ou em paralelo (um pedido independente para cada parte). Ela não foi copiada para cá, para as duas cópias não ficarem diferentes. Instale direto do repositório dela, seguindo o README de lá.

## Como instalar

Primeiro, baixe este repositório:

```bash
git clone https://github.com/marcel-grokbots/prumo-skills.git
cd prumo-skills
```

Depois copie as pastas de `skills/` para a pasta de skills da sua ferramenta. Os caminhos abaixo são os da documentação oficial de cada uma.

### Claude Code

Para todos os seus projetos:

```bash
mkdir -p ~/.claude/skills
cp -r skills/* ~/.claude/skills/
```

Só para um projeto: copie para `.claude/skills/` dentro da pasta do projeto.

Use pelo nome, por exemplo `/goal-pedido-com-prova`, ou deixe o Claude escolher a skill pelo assunto. Documentação: https://code.claude.com/docs/en/skills

### Codex

Para todos os seus projetos:

```bash
mkdir -p ~/.agents/skills
cp -r skills/* ~/.agents/skills/
```

Só para um repositório: copie para `.agents/skills/` dentro dele.

No Codex CLI ou na extensão para IDE, rode `/skills` ou digite `$` para chamar uma skill. Se ela não aparecer, reinicie o Codex. Documentação: https://developers.openai.com/codex/skills

### Cursor

Para todos os seus projetos:

```bash
mkdir -p ~/.cursor/skills
cp -r skills/* ~/.cursor/skills/
```

Só para um projeto: copie para `.cursor/skills/` ou `.agents/skills/` dentro dele. O Cursor também lê `~/.agents/skills/`, a mesma pasta do Codex.

No chat do Agent, digite `/` e procure o nome da skill. Documentação: https://cursor.com/docs/context/skills

## Estado das skills

Os prompts e exemplos destas skills ainda não passaram pelo teste com o público do Prumo. Os exemplos são ilustrativos. Confira sempre o resultado da IA antes de confiar nele.

## Quer ir além?

- O Prumo, curso completo de IA para o dia a dia: https://prumo.academy
- MSCREATIVE.SYSTEMS, o trabalho do Marcel Serrano com sistemas de IA: https://mscreative.systems

## Licença

MIT. Copyright (c) 2026 Marcel Serrano. Veja [LICENSE](LICENSE).
