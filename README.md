# Conhecendo Agentes de IA

Este conteúdo faz parte da mentoria do **"Bootcamp Santander 2025 - Automação com N8N"** na plataforma da **DIO**.

### O que são Agentes de IA?

De forma simples, um Agente de IA não é apenas um chat que responde perguntas. Pense nele como um "estagiário digital" que tem autonomia. Ele recebe um objetivo e tem permissão para usar ferramentas (como consultar o Google, ler um banco de dados ou enviar um e-mail) para realizar uma tarefa. O **n8n** atua como o escritório onde esse estagiário trabalha, conectando a inteligência da IA com os aplicativos que você usa no dia a dia.

---

## Formas de usar o [N8N](https://docs.n8n.io/)

Para acompanhar a mentoria e criar seus fluxos, você tem duas opções principais:

### 1. N8N Cloud (Online)

É a forma mais rápida de começar, sem precisar instalar nada. Você cria uma conta no site oficial e já sai usando.

* **Prós:** Não consome recursos do seu PC.
* **Contras:** É um serviço pago (possui um período de teste gratuito/free tier).

> [!NOTE]
> https://app.n8n.cloud

### 2. Instalação Local (Docker)

É a versão que roda diretamente na sua máquina. É gratuita e perfeita para estudos e automações pessoais. Foi a opção que escolhi para esta live. Se você já tem o Docker instalado, basta rodar os comandos abaixo no seu terminal para subir o container:

```bash
docker volume create n8n_data

docker run -it --rm --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
```

Após rodar o comando, acesse `http://localhost:5678` no seu navegador.

> [!NOTE]
> https://hub.docker.com/r/n8nio/n8n

---

## 📝 TODO: O Que Faremos na Live

Nosso objetivo prático será construir nosso primeiro Agente do zero.

* [ ] Criar um Agente de IA para auxiliar na resolução e entendimento dos **Desafios de Código** do Bootcamp.
