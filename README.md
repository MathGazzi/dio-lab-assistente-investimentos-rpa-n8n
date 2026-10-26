# 🤖 Assistente de Investimentos com RPA e n8n (DIO Lab)

Projeto desenvolvido para o desafio prático da [DIO](https://dio.me) unindo automação com Python (RPA) e orquestração de processos no n8n.

## 🎯 Objetivo
Automatizar a extração de dados de clientes a partir de uma página web simulada, processar os perfis de investidores (Conservador, Moderado e Arrojado) e gerar recomendações de investimento personalizadas baseadas nas opções disponíveis.

## 🛠️ Tecnologias Utilizadas
- **Python:** Script de RPA com BeautifulSoup e Requests para raspagem e envio dos dados.
- **n8n:** Orquestração de workflow via Webhook, processamento e cruzamento de dados.
- **HTML / CSV:** Bases de dados simuladas de clientes e ativos de investimento.

## 🚀 Como Funciona o Fluxo
1. O script Python (`src/extrair_clientes.ipynb` / `extrair.py`) coleta os clientes da página web.
2. Os dados são enviados via requisição HTTP POST para o Webhook do n8n.
3. O n8n baixa a base de investimentos (`data.csv`) e cruza o perfil de cada cliente.
4. São geradas mensagens personalizadas com templates baseados no perfil (foco em renda fixa para Conservador, equilíbrio para Moderado e ações para Arrojado).

## 📸 Evidência de Execução (MVP)
<img width="1327" height="358" alt="image" src="https://github.com/user-attachments/assets/a43dbb05-9e60-46f1-80e9-64e863a5cef1" />

<img width="680" height="623" alt="image" src="https://github.com/user-attachments/assets/d7c069ac-2ef3-4b5e-90c3-4ebb73ff1fc6" />

