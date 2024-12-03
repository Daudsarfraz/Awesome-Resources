<div align="center">

## Large Language Models as Zero-shot Dialogue State Tracker through Function Calling

Zekun Li, Zhiyu Zoey Chen, Mike Ross, Patrick Huber, Seungwhan Moon, Zhaojiang Lin, Xin Luna Dong, Adithya Sagar, Xifeng Yan, Paul A. Crook
<br>Arxiv submission available [here](https://arxiv.org/abs/2402.10466)</div>

---

Large language models (LLMs) are increasingly prevalent in conversational systems due to their advanced understanding and generative capabilities in general contexts. However, their effectiveness in task-oriented dialogues (TOD), which requires not only response generation but also effective dialogue state tracking (DST) within specific tasks and domains, remains less satisfying. In this work, we propose a novel approach FnCTOD for solving DST with LLMs through function calling. This method improves zero-shot DST, allowing adaptation to diverse domains without extensive data collection or model tuning. Our experimental results demonstrate that our approach achieves exceptional performance with both modestly sized open-source and also proprietary LLMs: with in-context prompting it enables various 7B or 13B parameter models to surpass the previous state-of-the-art (SOTA) achieved by ChatGPT, and improves ChatGPT's performance beating the SOTA by 5.6% Avg. JGA. Individual model results for GPT-3.5 and GPT-4 are boosted by 4.8% and 14%, respectively. We also show that by fine-tuning on a small collection of diverse task-oriented dialogues, we can equip modestly sized models, specifically a 13B parameter LLaMA2-Chat model, with function-calling capabilities and DST performance comparable to ChatGPT while maintaining their chat capabilities. We plan to open-source experimental code and model.

---

### 📑 Self Notes

O artigo inicia com um breve parágrafo sobre LLMs e apresenta o desafio que baseou seu estudo: o problema de modelos de linguagem serem capazes de responder bem em tipos de conversas `chat`. Conhecemos essas conversas como conversas comuns com chatbots, que temos o assistant (chatbot) e o usuário em um diálogo. Modelos conseguem responder bem em contextos gerais de pergunta-resposta (Q&A) por exemplo, mas não manter essas conversas.<br>

A partir disso, são apresentados dois termos que o artigo mencionará ao longo de seu desenvolvimento: `TOD - Task-oriented dialog` e `DST - Dialog State Tracker`. O diálogo orientado a tarefas é importante em um contexto conversacional porque 1) existem mensagens simultâneas que se perpetuam ao longo da conversa e 2) o modelo precisa saber identificar e extrair, para cada mensagem que o usuário envia, suas intenções.

`The challenge lies in the model's hability to accurately summarize user needs over multiple turns of conversation and also strictly adhere`





