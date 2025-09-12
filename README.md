Com certeza! Aqui está uma proposta de `README.md` bem estruturada e profissional para o projeto de vocês, em português do Brasil.

Você pode copiar e colar o texto abaixo diretamente em um arquivo chamado `README.md` no seu repositório do GitHub.

---

# Evolving Visions: Geração de Vídeo com Stable Diffusion

![Status](https://img.shields.io/badge/status-concluído-brightgreen)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)
![Framework](https://img.shields.io/badge/Framework-PyTorch-orange?logo=pytorch)
![Tool](https://img.shields.io/badge/Tool-Hugging_Face-yellow.svg)

Projeto desenvolvido para o Checkpoint 1 da disciplina de Visão Computacional, do 2º semestre do curso de Análise e Desenvolvimento de Sistemas da FIAP.

## ✒️ Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [🎥 Vídeo Gerado](#-vídeo-gerado)
- [🛠️ Tecnologias Utilizadas](#️-tecnologias-utilizadas)
- [🚀 Como Executar](#-como-executar)
- [🧩 Estrutura do Código](#-estrutura-do-código)
- [👥 Integrantes](#-integrantes)

## 📖 Sobre o Projeto

O objetivo deste projeto é criar uma animação em vídeo utilizando o modelo de inteligência artificial **Stable Diffusion**. A principal técnica empregada é um **loop de feedback**, onde cada quadro (frame) do vídeo é gerado a partir do quadro anterior.

O processo funciona da seguinte forma:
1.  **Frame Inicial:** Uma imagem é gerada a partir de um comando de texto (prompt) utilizando um pipeline *Text-to-Image*.
2.  **Frames Subsequentes:** A imagem gerada no passo anterior é retroalimentada no modelo, através de um pipeline *Image-to-Image*, para gerar o próximo frame.
3.  **Continuidade:** Esse processo é repetido dezenas ou centenas de vezes. Ao ajustar o parâmetro `strength` (força), controlamos o nível de alteração entre um frame e outro, criando uma animação fluida e contínua com um efeito de "morphing" ou "sonho".

O resultado é um vídeo que demonstra uma transição visual orgânica e fascinante, inteiramente gerada por IA.

## 🎥 Vídeo Gerado
[
*-- Insira aqui um GIF do seu vídeo ou um link para o YouTube! --*](https://youtube.com/shorts/noNJvpdIY68?feature=share)

**Exemplo de como inserir um GIF no README:**
`![Demonstração do Vídeo](link_para_o_seu_gif.gif)`

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python
- **Ambiente:** Google Colab
- **Bibliotecas Principais:**
  - `PyTorch`: Framework de Deep Learning.
  - `Diffusers`: Biblioteca da Hugging Face para interagir com modelos de difusão.
  - `Transformers`: Para carregar componentes do modelo.
  - `OpenCV (cv2)`: Para a montagem do vídeo final a partir dos frames.
  - `Pillow (PIL)`: Para manipulação de imagens.

## 🚀 Como Executar

O projeto foi desenvolvido em um notebook do Google Colab e pode ser facilmente reproduzido.

1.  **Abra o Notebook:**
    - [Link para o Google Colab]([https://colab.research.google.com/drive/SEU_LINK_AQUI](https://colab.research.google.com/drive/1MHIKbUlqu9NDIRcTOhKwqI3BsDPfVGRB?usp=sharing))  

2.  **Configure o Ambiente de Execução:**
    - No menu, vá em `Ambiente de execução` > `Alterar o tipo de ambiente de execução`.
    - Em `Acelerador de hardware`, selecione **GPU**. Isso é essencial para a execução do modelo.

3.  **Execute as Células:**
    - Execute a primeira célula para instalar todas as dependências (`!pip install ...`).
    - Execute a célula principal do código. Você pode customizar os parâmetros na seção **"DEFINA SUA ANIMAÇÃO"**, alterando o `prompt`, o número de frames (`num_frames`) e a força da transição (`strength`).

4.  **Resultados:**
    - Os frames gerados serão salvos na pasta `frames`, e o vídeo final (`video_gerado.mp4`) estará disponível para download no painel de arquivos do Colab.

## 🧩 Estrutura do Código

O código no notebook está dividido em 5 partes principais para facilitar o entendimento:

1.  **Instalação de Dependências:** Configuração inicial do ambiente.
2.  **Importações e Configuração:** Carregamento das bibliotecas e dos modelos pré-treinados (`runwayml/stable-diffusion-v1-5`).
3.  **Definição da Animação:** Seção onde os principais parâmetros criativos (prompt, frames, strength) são definidos.
4.  **Geração dos Frames:** O loop principal que cria a imagem inicial e, em seguida, itera para gerar os frames subsequentes.
5.  **Montagem do Vídeo Final:** Utiliza o OpenCV para compilar todas as imagens salvas em um arquivo de vídeo .mp4.

## 👥 Integrantes

| RM      | Nome Completo             |
| :------ | :------------------------ |
| 555762  | Ana Carolina Martins      |
| 555848  | Andre Rovai Jr            |
| 554707  | Lancelot Chagas Rodrigues |
| 555082  | Kauan Alves               |

---
