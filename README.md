# 🎙️ Lab de Pronúncia (labdepronuncia)

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

> Application to identify and provide pronunciation improvements for language learners.

O **Laboratório de Pronúncia Multilíngue** é uma ferramenta interativa desenvolvida para prática fonética avançada. Utilizando inteligência artificial de ponta, o sistema analisa sua fala e fornece feedbacks pedagógicos em tempo real.

---

## 🚀 Funcionalidades

- **Multilingue:** Suporte para Inglês, Alemão, Mandarim, Espanhol e Francês.
- **Análise com IA:** Feedback detalhado sobre entonação e fonética.
- **Captura In-Browser:** Sistema de captação de áudio via JavaScript integrado ao Colab.
- **V2 Features:** Opção de download dos feedbacks e áudios de referência (padrão nativo).

## 🛠️ Tecnologias e APIs

O projeto combina três pilares tecnológicos:
1. **Whisper (OpenAI):** Transcrição precisa do áudio capturado.
2. **Gemini (Google):** Inteligência analítica para avaliação pedagógica.
3. **gTTS (Google Text-to-Speech):** Síntese de voz nativa para referência.

---

## 📋 Pré-requisitos

Para rodar este laboratório, você precisará de:

1. **Google Colab:** Os scripts foram otimizados para rodar no [Google Colab](https://colab.research.google.com/) devido ao suporte nativo para áudio via navegador.
2. **API Key do Gemini:** É necessário gerar uma chave gratuita no [Google AI Studio](https://aistudio.google.com/app/apikey).

---

## ⚙️ Como Usar

1. Acesse o notebook no ambiente do Google Colab.
2. Insira sua `API_KEY` quando solicitado.
3. Selecione o idioma que deseja praticar.
4. Grave sua voz pronunciando a palavra ou expressão sugerida.
5. Receba a análise e baixe o áudio de referência para comparação (disponível na V2).

---


## 🔄 Fluxo de Funcionamento

Para entender como a mágica acontece por baixo do capô, aqui está o ciclo de processamento de cada prática:

1. **Captura de Áudio** (`JavaScript`)
   - O áudio é gravado diretamente do seu microfone através da API do navegador e enviado para o ambiente Python.
2. **Transcrição** (`Whisper by OpenAI`)
   - O modelo de IA processa o áudio e o transforma em texto, identificando exatamente o que foi dito.
3. **Análise Pedagógica** (`Gemini AI`)
   - O texto transcrito é enviado ao Gemini, que compara com a expressão correta e gera dicas de melhoria fonética.
4. **Síntese de Voz** (`gTTS`)
   - O sistema gera um áudio com pronúncia nativa para que você possa comparar sua fala com o padrão ideal.

**Diagrama de Processo:**
`Usuário` 🎙️ ➔ `JS Browser` ➔ `Whisper` ➔ `Gemini AI` ➔ `gTTS` ➔ 🎧 `Feedback`

---

## 🤝 Créditos e Referências

- **Autor:** [Felipe Oliveira](https://github.com/mecfoliveira86)
- **Inspiração:** Projeto desenvolvido originalmente durante o bootcamp da [DIO](https://www.dio.me/).

---
