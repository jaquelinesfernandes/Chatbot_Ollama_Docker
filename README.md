# 🐳💬 Chatbot Ollama com Docker 
Este projeto implementa um chatbot utilizando o modelo Ollama, com arquitetura modular baseada em containers Docker. 
A aplicação é composta por três camadas principais: Backend, API e Frontend.


## ⚙️Tecnologias Utilizadas
- **Backend**
  - FastAPI — Framework moderno para APIs em Python
  - Pydantic — Validação de dados e tipagem
  - Ollama — Execução local de modelos LLM
- **Frontend**
  - Streamlit — Interface web interativa para visualização e interação com a API
- **Infraestrutura**
  - Docker
  - Docker Compose

## 🚀 Como Executar

- Leia o arquivo LEIAME.txt

  1.Clone o repositório:

            git clone https://github.com/jaquelinesfernandes/Chatbot_Ollama_Docker
            cd Chatbot_Ollama_Docker

  2.Execute com Docker Compose:
  
            docker-compose up --build

  3.Acesse os serviços:
      - Frontend (Streamlit): http://localhost:8501
      - Backend (FastAPI docs): http://localhost:8000/docs
  
## 🧠 Ollama
O serviço Ollama é executado em um container separado e expõe uma API local para interação com modelos como LLaMA, Mistral, entre outros. O backend FastAPI se comunica com o Ollama via HTTP.

## 📂 Organização dos Containers
| Serviço  | Porta | Descrição                      |
|----------|-------|--------------------------------|
| Backend  | 8000  | API REST com FastAPI           |
| Frontend | 8501  | Interface Streamlit            |
| Ollama   | 11434 | Servidor de modelos LLLM local |

## 📌 Observações
- Certifique-se de que sua máquina possui suporte para execução de containers com acesso à GPU (opcional para modelos maiores).
- O Ollama precisa ser configurado com o modelo desejado no Dockerfile ou via comandos no container.




