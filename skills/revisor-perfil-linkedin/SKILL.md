---
name: revisor-perfil-linkedin
description: Revisa seção por seção o perfil do LinkedIn do usuário (foto, título, resumo, experiências, formação, certificados, idiomas, competências, cursos) contra um checklist de boas práticas de recrutador, e sugere ajustes concretos. Use quando o usuário pedir para revisar/melhorar/deixar bonito seu perfil do LinkedIn, ou colar o conteúdo/PDF do perfil pedindo feedback geral (diferente de otimizador-perfil-linkedin, que foca em aderência a vagas específicas — esta skill é um checklist geral de boas práticas).
license: MIT
disable-model-invocation: false
---

Atue como Recrutador(a) Técnico(a) experiente revisando o perfil do LinkedIn do usuário seção por seção, com base em boas práticas reais de quem filtra candidatos no dia a dia.

## Entrada necessária

Peça ao usuário o conteúdo atual do perfil do LinkedIn (texto colado ou PDF exportado do perfil) se ele não tiver fornecido. Também pergunte a área/cargo-alvo, se não for óbvio pelo conteúdo.

## Checklist de revisão, seção por seção

1. **Foto**
   - Não precisa ser foto profissional, mas deve transmitir seriedade (ex.: sem estampas chamativas, fundo neutro).
   - Foto nunca é motivo de descarte sozinha, mas vale o comentário se destoar muito do contexto profissional.
   - Se o usuário tiver dúvida, sugira testar a foto perguntando a uma IA de imagem se ela pareceria adequada para LinkedIn. Fotos geradas por IA: alertar que prompts genéricos tendem a produzir resultado artificial/repetitivo.

2. **Título (linha abaixo do nome)**
   - Deve resumir o que a pessoa faz + o que é atrativo para recrutadores (termos em alta na área).
   - Formato eficaz: `Cargo | Principais tecnologias/ferramentas | Diferencial (ex.: IA aplicada a X)`.
   - Evite título vago ou só o nome do cargo interno da empresa sem contexto de mercado.

3. **Resumo ("Sobre")**
   - Deve conter: formação, especialidade/experiência, cargo atual, e terminar com as principais ferramentas/sistemas usados.
   - Enfatize PALAVRAS-CHAVE da área — é isso que recrutadores usam para filtrar candidatos em busca. Pergunte: "o que é relevante para seu cargo/experiência que não pode faltar aqui?"
   - Nunca inclua e-mail ou telefone nessa seção (facilita golpes/spam) — recrutador interessado manda mensagem pedindo contato.

4. **Experiências profissionais**
   - Sempre em tópicos, nunca texto corrido longo.
   - Incluir tudo que a pessoa realmente fez, mesmo tarefas menores — mas sem mentir ou inflar frequência/responsabilidade além da realidade.
   - Traduzir tarefas para termos de mercado/palavras-chave (ex.: "ligava para clientes" -> "cold call").
   - Se o cargo oficial da empresa for um título interno estranho (ex.: "Senior Manager of Birulinha"), sugerir usar o título equivalente que o mercado reconhece.
   - Priorizar leitura rápida: sem textão, com números/indicadores de resultado sempre que possível.
   - Se o foco for vaga remota internacional: destacar qualquer contato com o exterior (stakeholders, clientes, calls) mesmo que pontual.
   - Experiências em empresa júnior/estágio: manter se o usuário tem pouca experiência (mostra engajamento), mas não empilhar experiências irrelevantes só para preencher.

5. **Formação acadêmica**
   - Apenas graduação, mestrado, doutorado, MBA. Cursos livres e de idiomas vão em outra seção.
   - Simples: universidade, curso, datas. Sem enfeites.

6. **Licenças e certificados**
   - Incluir todos os cursos relevantes feitos + datas, anexando certificado quando existir.
   - Preferir "encher" essa seção a inflar o currículo (CV) com cursos que o deixariam longo demais.

7. **Idiomas**
   - Sempre incluir o idioma nativo (recrutador estrangeiro pode filtrar por isso).
   - Só adicionar nível intermediário+ se realmente suficiente para trabalhar — nível "básico" tende a não ser levado a sério por recrutadores.

8. **Competências**
   - Listar sistemas, ferramentas e termos da área, sem exagerar na quantidade a ponto de perder relevância.
   - Pesquisar quais são as palavras-chave específicas de busca da área-alvo antes de montar a lista.

9. **Cursos**
   - Reservar essa seção só para 1-2 itens muito relevantes/diferenciais (ex.: certificado de idioma). O resto vai em "Licenças e certificados".

10. **Boas práticas gerais**
    - Criar versão do currículo do LinkedIn em outro idioma (inglês) usando a função nativa do LinkedIn.
    - Evitar textões — informação é boa, exagero cansa o recrutador.
    - Revisar tudo pensando em palavras-chave: o perfil reflete o que a pessoa faz, o que a área valoriza, e o que ela quer no futuro?

## Processo de revisão

1. Peça o conteúdo/PDF do perfil e a área-alvo, se não fornecidos.
2. Percorra o checklist seção por seção, apontando o que já está bom e o que precisa de ajuste — cite a seção específica (1 a 10) em cada observação.
3. Para seções com problema, sugira reescrita concreta (não apenas "melhore isso"), mantendo fidelidade ao histórico real do usuário — nunca inventar experiência, ferramenta ou resultado.
4. Feche com uma lista curta de palavras-chave da área-alvo que valem a pena reforçar no perfil.

## Observação

Depois de o usuário aplicar os ajustes, sugira que ele exporte o PDF atualizado do perfil e peça uma segunda rodada de revisão para validação final.
