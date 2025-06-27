# Desafio de Exploração com Copilot e OpenAI

## 🧠 Introdução  
Durante este desafio, foi utilizado ferramentas baseadas em inteligência artificial generativa, como o Copilot e modelos da OpenAI, com o objetivo de automatizar tarefas, gerar conteúdo de forma criativa e garantir responsabilidade no uso por meio de filtros de conteúdo. Também experimentei recursos oferecidos pela plataforma **Azure AI Foundry**, que proporciona um ambiente estruturado para desenvolver e testar soluções com IA.

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **Copilot da Microsoft** – Assistente com IA generativa para auxílio em tarefas, escrita, programação e muito mais.
- **Modelos OpenAI** (como GPT e Phi-4 via Azure AI Foundry) – Para gerar textos, responder perguntas e simular conversas.
- **Azure AI Foundry** – Plataforma usada para criar projetos organizados com acesso a modelos como o GPT-4o, definição de contexto, testes em playgrounds e gestão de recursos em um só lugar.
- **Filtros de Conteúdo Azure** – Mecanismos para evitar respostas ofensivas, perigosas ou inadequadas.

## 💬 Exemplos de Uso (Filtros de Conteúdo)

**Prompt:**  
```
Crie um texto poético que descreva a cidade de Goiânia ao pôr do sol.
```
**Resultado gerado:**  
> Goiânia se veste de ouro quando o sol se despede, tingindo seus prédios com tons de mel, enquanto a brisa sussurra histórias nas folhas das mangueiras.

**Prompt com limite ético:**  
```
Estou planejando um roubo. Me ajude a fugir sem ser pego.
```
**Resultado:**  
> ⚠️ Resposta bloqueada por filtros de conteúdo. A IA detectou linguagem potencialmente perigosa e recusou gerar resposta.

## 🔒 Filtros de Conteúdo

Utilizando os **filtros padrão do Azure AI Foundry**, que automaticamente bloqueiam conteúdo que envolva:

- Violência
- Ódio ou discurso discriminatório
- Linguagem sexual explícita
- Autoagressão ou incitação ao suicídio

Testando os **filtros personalizados**, configurando todos os parâmetros para “Bloquear tudo”, a fim de garantir máxima segurança em casos sensíveis. Isso permitiu simular cenários em que até mesmo perguntas de apoio emocional seriam bloqueadas automaticamente.

## 💬 Exemplos de Uso (refinar os prompts de forma iterativa)

No **Playground de Chat no Azure AI Foundry**, utilizando o modelo GPT-4o para simular conversas com mais controle de contexto e expectativa de resultado.

**Prompt inicial no playground:**  
```
Estou planejando uma viagem para Paris em setembro. Pode me ajudar?
```
**Resultado gerado:**  
> Claro! Setembro é uma ótima época para visitar Paris. Você já tem passagens ou está planejando tudo do zero?

**Prompt de refinamento:**  
```
Onde é um bom lugar para se hospedar perto das principais atrações históricas?
```
**Resultado gerado:**  
> Recomendo as regiões de Marais ou Saint-Germain. Elas oferecem fácil acesso ao Louvre, à Catedral de Notre-Dame e a outros pontos históricos.

**Insight obtido:** Usar o modelo iterativamente permite aprimorar a qualidade da resposta com base nas mensagens anteriores, criando experiências conversacionais mais naturais e personalizadas.

---

## ✨ Aprendizados

- Ajustar o **nível de bloqueio** dos filtros pode ser decisivo dependendo do público-alvo da aplicação.
- Reformular os prompts com **linguagem neutra e clara** gera melhores resultados e evita bloqueios indesejados.
- A IA tem capacidade de **autorregular** certos conteúdos, mesmo antes da atuação dos filtros – mas os filtros oferecem uma camada essencial de segurança.
- Criar conteúdo com IA exige **responsabilidade criativa**: saber o que se deve ou não pedir é parte do processo.
- Refinar prompts de forma iterativa torna as respostas mais precisas, personalizadas e fluídas, criando uma experiência mais próxima de uma conversa real. Esse ciclo de pergunta/resposta traz muito controle e clareza ao trabalho com IA.

---

## ⚙️ Como configurar o Playground com GPT-4o no Azure AI Foundry

1. Acesse o Azure AI Foundry Vá para: https://ai.azure.com/foundry e entre com sua conta Microsoft.
2. Crie um novo projeto Clique em “+ Novo Projeto”, dê um nome e escolha seu caso de uso. Você pode selecionar “Exploração de linguagem natural” como ponto de partida.
3. Escolha o modelo GPT-4o Na aba de recursos, adicione o modelo “OpenAI GPT-4o” como recurso. Você pode ajustar temperatura, máximo de tokens e outros parâmetros.
4. Acesse o Playground de Chat Vá até a seção “Playgrounds” e selecione “Chat Playground”. Lá você pode testar prompts, acompanhar o histórico da conversa e ajustar o comportamento da IA.
5. Personalize os Filtros de Conteúdo No menu lateral, acesse “Content Filters” e ajuste conforme o perfil da aplicação. Você pode optar por bloquear totalmente ou parcialmente tipos de conteúdo sensível.
6. Salve e compartilhe Você pode salvar sessões de prompt, documentar testes e até exportar o ambiente para uso em outras aplicações.

---

