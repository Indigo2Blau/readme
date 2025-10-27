# 💡 readme
# 👋 Oiê — sou o Giovanni (Indigo2Blau) 😄

Sou Prompt Engineer — crio, testo e melhoro prompts para LLMs. Aqui compartilho meus projetos, ideias, dicas de prompts e um pouco do que aprendo no dia a dia! 🚀

## TL;DR
- Trabalho com engenharia de prompts para produtos, automações e pesquisa.
- Experiência com GPT, Llama, Claude e frameworks tipo LangChain.
- Curto criar prompts robustos, templates práticos, avaliação automática e pipelines de fine-tuning/instrução.

---

## Sobre mim
Curioso por natureza, adoro transformar perguntas vagas em instruções super claras para LLMs 🤖. Gosto de medir resultados, evitar alucinações e criar experiências que realmente ajudam.

Meus interesses:
- Design de prompts e templates reutilizáveis 📝
- Prompt chaining & orquestração (multi-step) 🔗
- Avaliação automática e métricas de qualidade 📊
- Prompt engineering para produtos: chatbots, assistentes, geração de código, resumo, classificação 🤝
- Integração com pipelines (APIs, LangChain, agentes) 🔌

---

## Como eu penso e trabalho 👨‍💻
1. Defino o objetivo: o que o usuário precisa e como seria a saída perfeita.
2. Crio contexto: só o essencial, nada de informação demais.
3. Estruturo: divido em passos se precisar de raciocínio mais complexo.
4. Segurança: adiciono guardrails e verificações (sem toxicidade por aqui!).
5. Testes e métricas: faço casos de teste e acompanho os resultados.
6. Itero: ajusto instruções, temperatura, contexto, tudo pra ficar melhor!

---

## Skills & Ferramentas 🛠️
- Modelos: OpenAI GPT (3.5/4), Anthropic Claude, Meta Llama, etc.
- Frameworks: LangChain, PromptLayer, Guidance, Hugging Face pipelines
- Infra & APIs: OpenAI API, Azure OpenAI, Hugging Face Hub
- Extras: Vector DBs (Pinecone, Milvus), ferramentas de avaliação (BLEU, ROUGE, embedding similarity)
- Outras: Python, JS/TS, testes automatizados, GitHub Actions

---

## Exemplos de Prompt & Templates ✨
Resumo técnico direto:
```
Você é um assistente de resumo técnico. Receba o texto abaixo e entregue:
1) Um resumo em 3 frases (máx. 60 palavras).
2) Lista de 5 termos importantes com definições curtas.
3) Sugestão de 2 referências para leitura adicional.

Texto:
<<INSERIR_TEXTO_AQUI>>
```

Gerador de testes unitários (JS):
```
Sistema: Você é um gerador de testes unitários confiável.
Instrução: Leia o trecho de código JavaScript e gere testes unitários usando Jest. Inclua casos de sucesso e falha, mocks necessários e comentários explicando cada teste.
Código:
<<INSERIR_CODIGO_AQUI>>
Formato de saída: JSON com chaves: "tests" (arquivo .test.js), "mocks", "comentarios".
```

Prompt chaining (análise + ação):
Step 1: Extrair entidades
```
Leia o texto e extraia: {nome, data, ação solicitada, urgência}. Retorne JSON.
```
Step 2: Resposta personalizada
```
Use o JSON gerado para compor uma resposta formal para o cliente, tom profissional, até 120 palavras.
```

---

## Memes em GIFs! 😆

### 1. "This is Fine" 🔥🐶  
![This is Fine](https://media.giphy.com/media/ARSp9T7wwxNcs/giphy.gif)

### 2. "Doge" 🐶✨  
![Doge](https://media.giphy.com/media/ToMjGpO6uV0dHtb7sYX/giphy.gif)

### 3. "Surprised Pikachu" 😲⚡  
![Surprised Pikachu](https://media.giphy.com/media/wSSooF0fJM97W/giphy.gif)

### 4. "Deal With It" 😎🕶️  
![Deal With It](https://media.giphy.com/media/l0MYt5jPR6QX5pnqM/giphy.gif)

### 5. "Rickroll" 🎸  
![Rickroll](https://media.giphy.com/media/Vuw9m5wXviFIQ/giphy.gif)

---

## Boas práticas (resumão) 🏆
- Seja explícito: diga como quer o formato, limite e exemplos.
- Contexto: só o relevante, sem exageros.
- Few-shot para estilos específicos.
- Teste com vários inputs e edge cases.
- Avalie e registre as respostas automaticamente.
- Ajuste temperatura/penalidades para equilibrar criatividade e precisão.

---

## Projetos & Portfólio 🔥
- [prompt-tooling](https://github.com/Indigo2Blau/prompt-tooling) — biblioteca de templates e testes para avaliação de prompts.
- [conversational-agent](https://github.com/Indigo2Blau/conversational-agent) — agente modular para suporte técnico com logs e métricas.
- [docgen](https://github.com/Indigo2Blau/docgen) — geração automática de documentação a partir de commits e comentários.

---

## Como trabalho com clientes/times 🤝
- Workshops para definir intents e casos de uso.
- Prototipagem rápida: templates e testes em 1–2 sprints.
- Integração & monitoração: deploy + coleta de métricas e logs.
- Finetune / RLHF: preparo datasets e avaliações quando precisa.

---

## Bora conversar? 💬
- GitHub: [Indigo2Blau](https://github.com/Indigo2Blau)
- Twitter / X: [Indigo2Blau](https://twitter.com/Indigo2Blau)
- LinkedIn: [indigo2blau](https://www.linkedin.com/in/indigo2blau)

Última atualização: 2025-10-27
