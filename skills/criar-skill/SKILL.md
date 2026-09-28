---
name: criar-skill
description: Cria uma nova skill (SKILL.md) no formato do repositório de skills e explica como publicar no GitHub e instalar via npx. Use quando o usuário pedir para criar, escrever ou publicar uma skill, ou disser "nova skill", "criar skill", "guia de skill".
license: MIT
disable-model-invocation: false
---

# Criar uma skill

Gera uma skill pronta para publicar num repositório GitHub e instalar com `npx skills add`.

## Processo

1. **Entender a skill.** Se faltar algo, pergunte (uma rodada curta, máx. 4 perguntas):
   - O que ela faz e qual resultado entrega?
   - Quando deve ser ativada (gatilhos, frases do usuário)?
   - Qual processo seguir, passo a passo? Deve fazer perguntas antes?
   - Como deve ser o output (formato, tamanho, idioma)?
   - Ativação: automática (o modelo decide) ou só manual (`/nome-da-skill`)?
2. **Definir o nome.** kebab-case, minúsculo, sem espaços/acentos (ex: `mega-brain-com-copy-thief`). O nome da pasta = campo `name`.
3. **Escrever o `SKILL.md`** no formato abaixo.
4. **Salvar** em `skills/<nome>/SKILL.md` dentro do repositório de skills.
5. **Atualizar o `README.md`** da raiz com uma linha: nome, o que faz, quando usar.
6. **Dar os comandos de publicar e instalar** (seção final).

## Formato do SKILL.md

```markdown
---
name: <nome-em-kebab-case>
description: <o que a skill faz e quando deve ser usada>
license: MIT
disable-model-invocation: <true | false>
---

<direcionamento: processo a seguir, formato do output, se deve fazer perguntas>
```

### Campos do frontmatter

| Campo | Regra |
|---|---|
| `name` | Igual ao nome da pasta. kebab-case. |
| `description` | Duas coisas: **o que faz** + **quando usar**. É o que o modelo lê para decidir ativar. Inclua gatilhos concretos e frases que o usuário diria. |
| `license` | Padrão `MIT`. |
| `disable-model-invocation` | `true` = só ativa manualmente, escrevendo `/<nome>` no prompt. `false` (ou omitido) = o modelo pode ativar sozinho quando julgar relevante. Use `true` para skills com efeito colateral ou que só fazem sentido sob demanda. |

### Corpo da skill

- Imperativo e direto. Passos numerados para processos.
- Diga se deve **perguntar antes** de executar e o quê.
- Defina o **formato do output** (estrutura, tamanho, idioma, exemplo).
- Curto: se passar de ~100 linhas, mova detalhes para arquivos auxiliares na mesma pasta e referencie.
- Sem informação óbvia que o modelo já sabe.

## Estrutura do repositório

```
skills/                      <- nome do repo (ex: seuusuario/skills)
├── README.md                <- como + quando usar cada skill
└── skills/
    └── <nome-da-skill>/
        └── SKILL.md
```

Se o repositório ainda não existe: criar no GitHub com nome `skills` (ex: `seuusuario/skills`), com essa estrutura.

## Publicar

Só faça `git push` se o usuário pedir. Comandos:

```bash
git add .
git commit -m "add skill <nome-da-skill>"
git push
```

Basta ter **pelo menos uma skill** no repositório para qualquer pessoa instalar.

## Instalar

Uma skill específica:

```bash
npx skills add <usuario>/skills --skill <nome-da-skill>
```

Todas as skills do repo:

```bash
npx skills add <usuario>/skills
```

## Checklist antes de entregar

- [ ] Pasta e `name` idênticos, em kebab-case
- [ ] `description` diz o que faz **e** quando usar
- [ ] `disable-model-invocation` escolhido de propósito
- [ ] Corpo define processo, perguntas e formato do output
- [ ] Linha adicionada ao `README.md`
- [ ] Usuário recebeu os comandos de instalar com o nome real do repo/skill
