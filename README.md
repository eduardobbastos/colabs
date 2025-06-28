# 🎧📝 Transcrição Automática de Vídeo e Áudio com Whisper no Google Colab

Este notebook permite que você transcreva vídeos ou áudios automaticamente, seja por upload ou por link (URL), utilizando o modelo Whisper da OpenAI.  
Todos os arquivos gerados terão um **timestamp** no nome para evitar sobrescrições.

---

## 🚀 **Funcionalidades**

- Aceita arquivos de vídeo **(.mp4, .mov, .avi, etc.)** ou áudio **(.mp3, .wav, etc.)**
- Permite processar conteúdos de **URL** (YouTube, Vimeo, etc.)
- Extrai automaticamente o áudio do vídeo antes de transcrever
- Utiliza o **modelo Whisper (medium)** para transcrição em português
- Salva a transcrição em arquivo `.txt` pronto para download
- Gera nomes únicos para todos os arquivos com base no timestamp

---

## 🖥️ **Como usar no Google Colab**

1. **Abra o notebook no Google Colab**
2. **Execute a célula de instalação de pacotes** (basta clicar no botão ▶️)
3. **Rode a célula principal do código**
4. Siga as instruções:
   - Escolha se quer transcrever **vídeo** ou **áudio**
   - Escolha entre **upload de arquivo** ou **inserção de URL**
   - Aguarde o processamento e download do arquivo de transcrição

---

## 📁 **Nomenclatura dos Arquivos**

- Todos os arquivos gerados (vídeo, áudio extraído, transcrição) terão um **timestamp** no nome, ex:
  - `meuvideo_20240627_193105_audio.mp3`
  - `meuaudio_20240627_193240_transcription.txt`

---

## 📝 **Personalização**

- Para máxima qualidade, troque `medium` por `large` na linha:
  ```python
  model = whisper.load_model("medium")
