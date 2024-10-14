```markdown
# Detecção de Movimento em Vídeos com OpenCV

Este repositório contém um aplicativo em Python que utiliza a biblioteca OpenCV para detectar movimento em vídeos. O sistema destaca as áreas onde ocorre movimento e salva o resultado em um novo arquivo de vídeo. Além disso, exibe o vídeo processado em uma janela ajustada à resolução da tela do dispositivo.

## Funcionalidades

- Captura a resolução da tela do dispositivo para exibir o vídeo processado de forma adequada.
- Processa um vídeo frame a frame para detectar movimentos.
- Destaca as áreas de movimento em vermelho.
- Salva o vídeo processado em formato MP4.
- Exibe o vídeo processado em uma janela ajustada à tela.

## Requisitos

Antes de executar o código, certifique-se de ter instalado as seguintes dependências:

- **Python 3.x**
- **OpenCV**
- **NumPy**
- **Tkinter** (geralmente incluído com a instalação do Python)
```

- Você pode instalar as bibliotecas necessárias utilizando pip:

```bash
    pip install opencv-python numpy
```

## Como Usar

1. **Clone o repositório**:

   ```bash
   git clone https://github.com/AngelusRocha/Visao_Computacional-2024.2
   ```

2. **Prepare seu vídeo**:
   Coloque o vídeo que deseja processar na pasta `videos` (ou no caminho especificado no código).

3. **Edite o código** (opcional):

   - Altere o caminho do vídeo de entrada na função `main()` caso necessário:
     ```python
     video_path = "../videos/horizontal.mp4"
     output_path = "../videos/videoOutput.mp4"
     ```

4. **Execute o código**:

   - Se estiver usando Jupyter Notebook na pasta do projeto:

     ```bash
     jupyter notebook
     ```

     - Abra o arquivo `index.ipynb`.
     - Adicione uma nova célula e chame a função `main()`:
       ```python
       main()
       ```
     - Execute a célula (pressionando `Shift + Enter`).

   - Se estiver usando o terminal:
     - Converta o notebook para um script Python:
       ```bash
       jupyter nbconvert --to script index.ipynb
       ```
     - Execute o script gerado:
       ```bash
       python index.py
       ```

5. **Visualize o resultado**:
   O vídeo processado será salvo no caminho especificado e exibido automaticamente na tela.

## Estrutura do Código

- **obter_resolucao()**: Captura a resolução da tela do dispositivo.
- **exibir_video(video_path)**: Lê e exibe o vídeo no caminho especificado.
- **processar_e_salvar_video(video_path, output_path, codec='XVID', fps=30)**: Processa o vídeo para detectar movimento e salva o resultado.
- **main()**: Ponto de entrada do aplicativo que orquestra o processamento e exibição do vídeo.

## Licença

Este projeto está licenciado sob a MIT License - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
