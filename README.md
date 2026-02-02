Projeto Assistente de Voz
Descrição  
Pequeno protótipo que integra Whisper (STT) → ChatGPT (NLP) → gTTS (TTS) para conversas por voz em pt-BR. Feito para rodar no Google Colab.

Requisitos

Python 3.10+ (no Colab já disponível)

Variável de ambiente: OPENAI_API_KEY

Principais bibliotecas: openai, pydub, gtts, soundfile

Como usar (Colab — resumo)

Instale dependências:

bash
!pip install openai pydub gtts soundfile
Defina a chave:

python
import os
os.environ["OPENAI_API_KEY"] = "SUA_CHAVE_AQUI"
Grave no navegador (JS) e faça upload do arquivo.

Converta para WAV (16 kHz mono) e transcreva com Whisper via API.

Envie a transcrição ao ChatGPT e gere áudio com gTTS.

Estrutura sugerida

notebook.ipynb — demo Colab pronto

README.md — instruções

requirements.txt — dependências

Boas práticas

Evite enviar dados sensíveis à API.

Teste com áudios curtos para reduzir custo.

Use Whisper local se precisar de privacidade.

Licença  
MIT
