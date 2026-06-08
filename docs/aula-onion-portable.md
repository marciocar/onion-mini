# Roteiro de Slides Detalhado: Ensinando o Onion Portable 🧅
*Guia do Instrutor — Curso Desenvolvimento com IA 2026 (Pulse Mais)*

Este documento serve como a base de conteúdo, visual e roteiro de fala para criar os slides de aula do **Onion Portable**. O objetivo pedagógico é ensinar aos alunos o paradigma de **Spec-as-Code** e como usar IAs de forma disciplinada.

---

## Slide 1: Capa do Treinamento
*   **Título Principal:** Onion Portable: O Poder do Spec-as-Code
*   **Subtítulo:** Metodologia de Desenvolvimento Disciplinado de Software com Inteligência Artificial
*   **Identidade Visual:** Fundo escuro (Dark Tech), logo com um gradiente roxo/azul-indigo com ícone de cebola minimalista.
*   **Rodapé:** Pulse Mais | Curso Desenvolvimento com IA 2026
*   **Notas do Instrutor:**
    > *"Boas-vindas a todos os alunos da Pulse Mais! Hoje vamos falar sobre a diferença entre gerar código descontroladamente e construir software de verdade utilizando IAs. Vamos introduzir o conceito de Spec-as-Code usando o Onion Portable: um framework leve projetado para rodar tanto no seu navegador comum quanto na sua IDE."*

---

## Slide 2: O Caos do Desenvolvimento com "1 Clique"
*   **Título:** A Crise da Geração Direta de Código
*   **Elementos Visuais:**
    *   Lado Esquerdo: Ícone de aviso (vermelho) com o prompt: *"Crie um sistema de reservas de hotel"*.
    *   Lado Direito: Uma avalanche de códigos desconexos, bugs de adivinhação, sem testes e sem documentação.
*   **Pontos de Destaque (Bullet Points):**
    *   **A Ilusão da Velocidade:** Gerar arquivos de código direto no início parece rápido, mas gera dívida técnica imediata.
    *   **Adivinhação de Requisitos:** Sem regras claras, a IA alucina regras de negócio, limites e APIs.
    *   **Falta de Âncora:** A IA perde a memória do contexto rapidamente à medida que o chat cresce.
*   **Notas do Instrutor:**
    > *"Quem nunca abriu o ChatGPT e pediu para ele escrever um código completo? No começo, parece mágico. Mas logo a IA começa a errar a arquitetura, esquecer as regras anteriores e criar bugs difíceis de rastrear. O erro não é da IA, é do nosso fluxo de trabalho. Sem uma âncora de especificação escrita antes do código, a IA fica sem norte."*

---

## Slide 3: O Paradigma Spec-as-Code (Especificação como Código)
*   **Título:** O que é Spec-as-Code?
*   **Elementos Visuais:**
    *   Fluxograma linear: **Ideia** ➔ 📑 **Especificação de Negócio** ➔ ⚙️ **Plano de Engenharia** ➔ 💻 **Código-Fonte**.
*   **Pontos de Destaque:**
    *   **Documentação Ativa:** As decisões de negócio e arquitetura técnica são salvas em arquivos Markdown no próprio repositório.
    *   **A Verdade Única:** A IA lê a especificação existente antes de sugerir ou editar o código.
    *   **Desenvolvimento Tridimensional:**
        1.  *Produto:* O que construir e por quê.
        2.  *Engenharia:* Como construir com padrões e qualidade.
        3.  *Compliance:* A validação de que o código implementou exatamente o planejado.
*   **Notas do Instrutor:**
    > *"A metodologia Spec-as-Code significa tratar a documentação de produto e técnica com a mesma importância e rigor que o código fonte. Eles vivem no repositório. A IA só escreve código se a especificação correspondente estiver aprovada."*

---

## Slide 4: O "Cérebro" Onion Portable
*   **Título:** Como funciona o Onion Portable?
*   **Elementos Visuais:**
    *   Desenho de uma Cebola com camadas: Camada externa (Negócio), Camada média (Técnico), Núcleo (Código).
*   **Pontos de Destaque:**
    *   **O Master Prompt:** O arquivo `ONION-MASTER-PROMPT.md` atua como o sistema operacional lógico da IA. Ele a impede de codificar imediatamente e a instrui a gerenciar as personas.
    *   **Otimizado para Limitações:** Reduzido de 6 para apenas **3 arquivos principais** para caber na restrição de 5 arquivos do plano grátis do ChatGPT.
*   **Notas do Instrutor:**
    > *"O Onion Portable foi desenhado para ser portátil. Ele condensa todo o poder do ecossistema Onion em 3 arquivos Markdown simples. Isso permite que qualquer aluno, mesmo em contas gratuitas de IA, possa utilizar a metodologia."*

---

## Slide 5: A Tríade Minimalista de Arquivos
*   **Título:** Os 3 Arquivos Pilares do Repositório
*   **Elementos Visuais:**
    *   Três ícones de arquivos estilizados lado a lado.
*   **Estrutura de Arquivos:**
    1.  `docs/business-context-lite.md` — **Contexto de Negócio:** Visão do produto, dores do cliente, backlog de features e regras de negócio ativas.
    2.  `docs/technical-context-lite.md` — **Contexto Técnico:** Stack tecnológica, padrões de código e os planos de implementação de engenharia passo a passo.
    3.  `docs/onion-cycles.md` — **As Regras dos Ciclos:** Guia de instruções centralizado que ensina as regras detalhadas de cada ciclo de persona (Produto, Engenharia, KB e Sincronismo).
*   **Notas do Instrutor:**
    > *"Estes são os únicos três arquivos de controle que você precisa colocar no seu repositório. Eles são pequenos, diretos e contêm o estado atual da verdade do seu projeto. A IA lê e atualiza esses arquivos conforme o desenvolvimento avança."*

---

## Slide 6: A Persona @product (O Ciclo de Produto)
*   **Título:** @product — Especificando o Negócio
*   **Elementos Visuais:**
    *   Ícone de quadro de post-its / produto.
*   **Fluxo de Trabalho:**
    *   **Fase de Coleta (Collect):** O usuário traz a ideia. O `@product` valida com as dores do cliente e refina em até 3 perguntas.
    *   **Fase de Especificação (Spec):** Escreve Histórias de Usuário, Critérios de Aceite testáveis e Regras de Negócio.
    *   **Fase de Consolidação:** Atualiza a seção 'Especificações Ativas' do `business-context-lite.md` e joga a feature no backlog como "Pronto para Dev".
*   **Notas do Instrutor:**
    > *"Quando o usuário tem uma ideia, a IA assume a persona de líder de produto (@product). Ela não vai programar nada nessa fase! Ela vai coletar os requisitos e documentar no arquivo de negócio. O código só inicia quando o negócio estiver definido."*

---

## Slide 7: A Persona @engineer (O Ciclo de Engenharia)
*   **Título:** @engineer — O Plano Arquitetural
*   **Elementos Visuais:**
    *   Ícone de régua/esquadro de engenharia e blocos de código.
*   **Fluxo de Trabalho:**
    *   **Fase de Início (Start):** Lê as especificações de negócio e o contexto técnico.
    *   **Fase de Planejamento (Plan):** Cria um plano de implementação detalhado (arquivos a criar/alterar + checklist lógico) no `technical-context-lite.md` e pede aprovação do usuário.
    *   **Fase de Execução (Work):** Escreve o código de forma incremental e marca cada item concluído no checklist.
*   **Notas do Instrutor:**
    > *"Uma vez especificado o produto, a IA muda de chapéu e assume a persona `@engineer`. Ela desenha o plano técnico e só programa depois que você aprovar esse plano. Isso evita refatorações desnecessárias no meio do caminho."*

---

## Slide 8: As Personas de Apoio: @meta & @docs
*   **Título:** @meta & @docs — Pesquisa e Sincronismo
*   **Elementos Visuais:**
    *   Duas colunas: Lado esquerdo (@meta), Lado direito (@docs).
*   **Funções Principais:**
    *   **@meta (Ciclo Knowledge Base):** Cria documentações profundas (`docs/knowledge-base/`) sobre APIs ou bibliotecas externas para ensinar a equipe e a IA.
    *   **@docs (Ciclo de Sincronismo / Sync):** Faz a engenharia reversa de códigos legados e preenche retroativamente os arquivos de contexto técnico e de negócio.
*   **Notas do Instrutor:**
    > *"A persona `@meta` é ótima para estudar novos conceitos e APIs difíceis. A persona `@docs` resolve a dor de quando já temos um código legado pronto e precisamos gerar a documentação de contexto Onion do zero."*

---

## Slide 9: Regra de Ouro (Invariante) & Bloqueio de Bypass
*   **Título:** O Guardião do Fluxo: Impedindo Atalhos
*   **Elementos Visuais:**
    *   Sinal de pare com uma cebola desenhada.
*   **A Regra Fundamental:**
    *   **Invariante:** Nunca gerar código funcional antes de documentar o produto e planejar a engenharia.
    *   **Bloqueio de Bypass:** Se você pedir código de forma afobada, o Onion Portable interrompe com um aviso de auto-consciência.
    *   **Auto-Diagnóstico:** O comando `/status` ou `/health` varre a pasta `docs/` e valida a consistência de todo o repositório.
*   **Notas do Instrutor:**
    > *"O Onion Portable possui um mecanismo de defesa. Se você tentar pular etapas pedindo o código diretamente, ele vai te dar um alerta amigável de bypass. Você pode forçar se quiser, mas o framework te lembrará de manter a disciplina para não gerar lixo."*

---

## Slide 10: Cenários de Execução (A vs. B)
*   **Título:** Cenário A (Web Chats) vs. Cenário B (IDEs Agênticas)
*   **Elementos Visuais:**
    *   Lado A (Navegador com Web Chat): Entrega de ZIPs e blocos de código.
    *   Lado B (IDE com terminal): Automação de escrita de arquivos em disco.
*   **Detecção Inteligente:**
    *   **Cenário A (Claude/ChatGPT):** A IA gera arquivos em blocos de markdown. No ChatGPT (com Code Interpreter), a IA roda scripts em Python para compactar todo o projeto em um arquivo `.zip` e disponibilizar link de download direto.
    *   **Cenário B (Antigravity/Cursor/Claude Code):** A IA detecta as ferramentas locais (`write_to_file`, etc.) e altera os contextos e códigos na máquina do usuário sem precisar de cópias manuais.
*   **Notas do Instrutor:**
    > *"Se você estiver no chat web do ChatGPT ou Claude, a IA adaptará a entrega dos arquivos Markdown. Ela se oferece para compactar a estrutura em ZIP para download (via Python/Code Interpreter) ou exibir artefatos individuais. Se estiver em IDEs agênticas como Cursor ou Antigravity, ela assume a escrita direta na máquina."*

---

## Slide 11: Demo Prática (Hands-on)
*   **Título:** Demonstração Prática do Fluxo
*   **Elementos Visuais:**
    *   Um mockup de tela mostrando o terminal e o navegador.
*   **Passo a Passo da Demonstração:**
    1.  Fazer upload do `ONION-MASTER-PROMPT.md` e dos 3 arquivos de contexto no ChatGPT ou Claude.
    2.  Lançar a ideia: *"Quero criar um botão de exportar para Excel"*.
    3.  Acompanhar a IA assumindo o `@product` e atualizando o `business-context-lite.md`.
    4.  Aprovar a especificação de produto.
    5.  Acompanhar o `@engineer` gerando o checklist técnico no `technical-context-lite.md`.
    6.  Autorizar a codificação e ver o resultado limpo e alinhado.
*   **Notas do Instrutor:**
    > *"Agora vamos abrir o ChatGPT ou a nossa IDE e assistir ao fluxo acontecer ao vivo. Vocês vão notar como a conversa ganha uma qualidade incrível quando a IA atua seguindo esse funil de disciplina."*

---

## Slide 12: Conclusão & Desafio Pulse Mais
*   **Título:** Torne-se o Arquiteto do Fluxo
*   **Elementos Visuais:**
    *   Ícone de troféu e gradiente Pulse Mais.
*   **Mensagem Final:**
    *   Código barato e rápido é commodity. O valor está em guiar a IA de forma arquitetada.
    *   **O Desafio:** Suba o Onion Portable em um repositório pessoal, execute o bootstrap, crie uma feature completa seguindo os ciclos e publique no seu portfólio.
*   **Notas do Instrutor:**
    > *"Escrever código qualquer IA faz hoje em dia. O que diferencia vocês como alunos da Pulse Mais em 2026 é a capacidade de arquitetar o fluxo de desenvolvimento de software e liderar a IA de ponta a ponta de forma escalável e com zero alucinações. Usem o Onion Portable nos seus desafios e projetos práticos. Muito obrigado!"*
