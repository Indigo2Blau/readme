# readme
# 👋 Olá — eu sou Giovanni (Indigo2Blau)

Sou Prompt Engineer — especialista em projetar, testar e otimizar prompts para modelos de linguagem (LLMs). Aqui no meu perfil compartilho meu trabalho, abordagens, exemplos práticos de prompts e recursos que uso para transformar intenções humanas em resultados consistentes e úteis com IA.

## TL;DR
- Atuo com engenharia de prompts para produtos, automações e pesquisa.
- Trabalho com modelos como GPT, Llama, Claude e frameworks como LangChain.
- Foco em prompts robustos, templates reutilizáveis, avaliação automática e pipelines de fine-tuning / instrução quando necessário.

---

## Sobre mim
Trabalho com interação entre humanos e modelos de linguagem: transformar requisitos vagos em instruções claras e confiáveis para LLMs. Gosto de medir resultados, reduzir alucinações e criar experiências previsíveis para usuários e sistemas automatizados.

Principais interesses:
- Design de prompts e templates reutilizáveis
- Prompt chaining e orquestração (multi-step)
- Avaliação automática e métricas de qualidade de resposta
- Prompt engineering para produtos (chatbots, assistentes, geração de código, resumo, classificação)
- Integração com pipelines (APIs, LangChain, agentes)

---

## Abordagem / Metodologia
1. Definição do objetivo: o que o usuário precisa e qual é a saída ideal.
2. Contexto: preparo de contexto minimalista e relevante (few-shot, system messages, instruções explícitas).
3. Estruturação: decompor em passos (prompt chaining) quando for necessário raciocínio composto.
4. Segurança e restrições: adicionar guardrails, verificação de toxicidade e limites de formato.
5. Testes e métricas: criar casos de teste, métricas de precisão/relevância e monitoramento em produção.
6. Iteração: coletar falhas, ajustar temperatura, truncamento de contexto e instruções.

---

## Skills & Ferramentas
- Modelos: OpenAI GPT (3.5/4), Anthropic Claude, Meta Llama, etc.
- Frameworks: LangChain, PromptLayer, Guidance, Hugging Face pipelines
- Infra & APIs: OpenAI API, Azure OpenAI, Hugging Face Hub
- Auxiliares: Vector DBs (Pinecone, Milvus), ferramentas de avaliação (BLEU, ROUGE, embedding similarity)
- Outras: Python, JavaScript/TypeScript, testes automatizados, GitHub Actions

---

## Projetos públicos
prompt-tooling  
[![CI]((https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExN2ZtZm9qN2VwaWV0bThicDJubzJxZHM5eGd4emlvZGxjN3J6Z3V1MSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/7ydUQC0CC2cNVtcrYH/giphy.gif))](https://github.com/Indigo2Blau/prompt-tooling) 
https://github.com/Indigo2Blau/prompt-tooling

conversational-agent  
[![Deploy]([https://media.giphy.com/media/3oEjI6SIIHBdRxXI40/giphy.gif](https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExbmRmOHlzZHduMGh5bzVmeTF4dXJrNmI0bTNlMmR2cjk1NXdycnR4YSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/CVtNe84hhYF9u/giphy.gif))](https://github.com/Indigo2Blau/conversational-agent)  
https://github.com/Indigo2Blau/conversational-agent

docgen  
[![Coverage]([https://media.giphy.com/media/l0HlQ7LRalxC6p8Ew/giphy.gif](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExaXlqMzRhaTlzcW0yZ3ZkMDRnNHFndHNlY2VpNzczcnNmMHF5ZXBiMiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/TEG31yxFAmJShqkcV3/giphy.gif))](https://github.com/Indigo2Blau/docgen) 
https://github.com/Indigo2Blau/docgen

---

## Templates & Exemplos de Prompt
Exemplo: Resumo técnico direto
```
Você é um assistente de resumo técnico. Receba o texto abaixo e entregue:
1) Um resumo em 3 frases (máx. 60 palavras).
2) Lista de 5 termos importantes com definições curtas.
3) Sugestão de 2 referências para leitura adicional.

Texto:
<<INSERIR_TEXTO_AQUI>>
```

Exemplo: Gerador de testes unitários (para JS)
```
Sistema: Você é um gerador de testes unitários confiável.
Instrução: Leia o trecho de código JavaScript e gere testes unitários usando Jest. Inclua casos de sucesso e falha, mocks necessários e comentários explicando cada teste.
Código:
<<INSERIR_CODIGO_AQUI>>
Formato de saída: JSON com chaves: "tests" (arquivo .test.js), "mocks", "comentarios".
```

Exemplo: Prompt chaining (análise + ação)
Step 1: Analisar e extrair entidades
```
Leia o texto e extraia: {nome, data, ação solicitada, urgência}. Retorne JSON.
```
Step 2: Gerar resposta personalizada com base no JSON
```
Use o JSON gerado para compor uma resposta formal para o cliente, tom profissional, até 120 palavras.
```

---

## Boas práticas (resumidas)
- Seja explícito: especifique formato de saída, limites e exemplos.
- Forneça contexto relevante, não todo o contexto possível.
- Use few-shot quando quiser um estilo específico.
- Teste com diversidade de inputs e edge cases.
- Automatize avaliação e logging das respostas.
- Controle temperatura e penalidades para equilíbrio entre criatividade e precisão.

---

## Projetos & Portfólio (destaques)
- prompt-tooling — biblioteca de templates e testes para avaliação de prompts. — https://github.com/Indigo2Blau/prompt-tooling
- conversational-agent — agente modular para suporte técnico com logs e métricas. — https://github.com/Indigo2Blau/conversational-agent
- docgen — geração automática de documentação a partir de commits e comentários de código. — https://github.com/Indigo2Blau/docgen

---

## Como trabalho com clientes / times
- Workshops iniciais para definição de intents e casos de uso.
- Prototipagem rápida: criar prompt templates e tests em 1–2 sprints.
- Integração e monitoramento: deploy da solução + coleta de métricas e logs.
- Finetune / RLHF: quando necessário, preparo datasets e avaliações.

---

## Contato
- GitHub: https://github.com/Indigo2Blau
- Twitter / X: https://twitter.com/Indigo2Blau
- LinkedIn: https://www.linkedin.com/in/indigo2blau

Última atualização: 2025-10-27
