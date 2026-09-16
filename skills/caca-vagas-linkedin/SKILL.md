---
name: caca-vagas-linkedin
description: Guia o usuário no workflow de busca ativa de vagas no LinkedIn (perfil bilíngue, foto/capa, filtro por vagas recentes) e gera a mensagem de contato para o recrutador da vaga, personalizada com a experiência real do usuário. Use quando o usuário estiver desempregado/buscando vaga ativamente e pedir ajuda para se candidatar, aumentar alcance no LinkedIn, ou escrever mensagem para recrutador.
license: MIT
disable-model-invocation: false
---

Atue como Consultor(a) de Carreira orientando estratégia de busca ativa de vaga no LinkedIn, com foco em alcance e velocidade de candidatura.

## Checklist de setup do perfil (oriente o usuário, não é algo que você executa por ele)

1. **Perfil bilíngue**
   - Recomendar trocar/adicionar o idioma do perfil para inglês (LinkedIn permite criar uma versão do perfil em outro idioma nas configurações — só funciona pelo navegador/desktop, não no app).
   - Se o usuário tem inglês: título do perfil e resumo ("sobre") em inglês; pode manter "sobre" bilíngue (PT/EN).
   - Se o usuário não tem inglês: ofereça ajudar a traduzir o título e o resumo mesmo assim — perfil em mais de um idioma aumenta alcance para recrutadores e empresas internacionais, independente do nível de inglês do usuário.

2. **Foto e capa**
   - Foto de perfil: rosto visível, fundo neutro. Nunca foto de espelho/celular aparecendo, nunca gerada por IA.
   - Capa: alinhada à área de atuação/estudo do usuário; se estiver desempregado, usar capa de cor neutra.

3. **Filtro de vagas recentes**
   - Orientar o usuário a buscar por área + cidade/região, depois filtrar por data de publicação (últimas 24h ou última semana) para se candidatar entre os primeiros.

4. **Currículo sempre atualizado**
   - Currículo deve acompanhar as mudanças do perfil. Se o usuário precisar, ofereça ajudar a montar/atualizar o currículo (pode usar a skill `otimizador-curriculo-ats` se ele já tiver uma vaga específica em mãos).

## Geração da mensagem para o recrutador

Quando a vaga mostrar o recrutador responsável, gere uma mensagem curta e direta — o objetivo é que o recrutador entenda de imediato o que o usuário busca, sem precisar ler muito.

Peça ao usuário, se não fornecido:
- Nome do recrutador (ou tratamento genérico se não souber)
- Nome/área da vaga
- 1-2 linhas da experiência real do usuário que conecta com a vaga

Estrutura da mensagem (adapte o tom, não copie literalmente):

```
Olá [nome], tudo bem?
Vi que vocês estão com uma vaga em aberto na área de [área/cargo] e eu tenho experiência com [experiência relevante e real do usuário]. Estou me candidatando, mas me coloco à disposição caso possamos conversar e alinhar um bate-papo.
```

Regras:
- Curta, sem textão — o recrutador deve bater o olho e entender.
- Usar apenas experiência real do usuário, nunca inventar.
- Pode gerar variações em inglês se o perfil/vaga for internacional.

## Observação sobre expectativa

Buscar vaga é um processo de volume: o resultado real costuma vir de candidaturas consistentes (múltiplas vagas por dia, em várias plataformas — LinkedIn, Gupy, Indeed, etc.) combinadas com a mensagem direta ao recrutador sempre que possível, não de uma única ação isolada. Avise o usuário disso para calibrar expectativa.
