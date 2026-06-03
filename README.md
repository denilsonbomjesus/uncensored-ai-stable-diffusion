# 🎨 Stable Diffusion – Geração de Imagens com CyberRealistic V8

Este repositório contém um **notebook Jupyter** configurado para rodar no **Google Colab** com aceleração GPU (T4). Ele utiliza o modelo **CyberRealistic V8 (FP16)** para gerar imagens fotorrealistas a partir de texto (text‑to‑image) e também para modificar imagens existentes (image‑to‑image).

## 🔍 Conteúdo

- `uncensored-ai-stable-diffusion.ipynb` – notebook principal com dois scripts:
  1. **Gerar imagem do zero (Text‑to‑Image)**
  2. **Modificar uma imagem existente (Image‑to‑Image)**

## 🚀 Como usar

### 1. Abrir no Google Colab

Faça o upload do notebook para o Google Colab ou acesse‑o diretamente pelo GitHub (se já corrigido).  
No Colab, ative a GPU:  
**Ambiente de execução → Alterar tipo de ambiente de execução → GPU (T4)**.

### 2. Executar o primeiro script – Gerar imagem do zero

- O notebook instala automaticamente as bibliotecas necessárias (`diffusers`, `transformers`, `accelerate`, `torch`).
- Baixa o modelo `stablediffusionapi/cyberrealistic` (aproximadamente 4 GB).
- Altere o `prompt` e o `negative_prompt` na célula indicada.
- Execute a célula – a imagem será salva como `imagem_gerada_do_zero.png` e exibida na saída.

**Exemplo de prompt** (inglês para melhores resultados):

```python
seu_prompt_aqui = "A cinematic portrait of a cyberpunk hacker sitting in a dark room, neon lights illuminating their face, highly detailed skin texture, 8k resolution, photorealistic"
