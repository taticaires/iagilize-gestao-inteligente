# IAgilize | Gestão Inteligente de Demandas

## Sobre o projeto

O IAgilize é uma **Prova de Conceito (POC) acadêmica** que explora o uso de Inteligência Artificial Generativa e Processamento de Linguagem Natural (NLP) para apoiar profissionais autônomos, inicialmente com foco em Social Media.

A proposta é interpretar mensagens de clientes, identificar informações relevantes (cliente, serviço, prazo e valor) e organizar a solicitação como uma tarefa em um painel demonstrativo.

## Funcionalidades demonstradas

- Interpretação de mensagens com a API Gemini.
- Extração estruturada de cliente, plano/serviço, demanda, prazo e valor.
- Classificação simplificada entre consulta/orçamento e contratação.
- Registro de demandas em uma lista mantida em memória.
- Cálculo demonstrativo de receitas previstas.
- Interface conversacional construída com Gradio.

## Tecnologias

- Python
- Google Gemini API (`google-genai`)
- Gradio
- JSON
- Google Colab

## Como executar no Google Colab

1. Abra `IAgilize_Gestao_Inteligente.ipynb` no Google Colab.
2. No painel lateral **Secrets** (ícone de chave), adicione `GEMINI_API_KEY` com uma chave válida do Google AI Studio.
3. Habilite o acesso ao segredo para o notebook.
4. Execute as células em ordem.
5. Teste uma mensagem usando os exemplos da interface.

**Nunca coloque sua chave de API diretamente no código ou em arquivos publicados.** Se uma chave já foi exposta, revogue-a e crie outra.

## Limitações desta POC

- Os registros são mantidos apenas em memória e são perdidos ao reiniciar a sessão.
- O fluxo de WhatsApp é apenas uma resposta sugerida na interface. Não existe integração real com WhatsApp.
- Os valores do catálogo são exemplos definidos para a demonstração, não uma tabela comercial vigente.
- A classificação de orçamento/contratação é simplificada e precisa de validação humana antes de qualquer decisão financeira.
- A interpretação depende da resposta gerada pelo modelo e pode conter erros.

## Contexto

Projeto apresentado como prova de conceito de uma solução de IA para organização de demandas de profissionais autônomos. A apresentação da solução descreve o problema, os objetivos, as tecnologias e o fluxo proposto.

## Estrutura

- `IAgilize_Gestao_Inteligente.ipynb`: notebook principal.
- `requirements.txt`: dependências Python.
