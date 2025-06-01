# Desenvolvimento de Aplicações Distribuídas
Repositório para publicação das resoluções dos exercícios de Laboratório das disciplinas de programação da PUC Minas!

## Alunos integrantes da equipe

* João Vitor Pedersoli Rajão
* Arthur Henrique Porto Silva
* Pedro Afonso De Campos Faria Maciel
* Miguel Pedrosa do Carmo Nonato
* Pedro Reis de Souza

## Professor responsável

* Nome completo do professor

## Instruções de Uso

O repositório do projeto contém a maior parte dos experimentos e análises em arquivos Jupyter Notebook (`.ipynb`), que permitem visualização interativa dos resultados e execução célula a célula. Para abrir e rodar esses notebooks, recomendamos utilizar o Visual Studio Code (VS Code) com a extensão **Jupyter** instalada, ou utilizar plataformas como Google Colab ou Jupyter Lab.

Para reproduzir os experimentos:

1. **Instale o Python (>=3.8)** e, preferencialmente, crie um ambiente virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate    # Linux/macOS
   venv\Scripts\activate       # Windows
   ```

2. **Instale as dependências** listadas nos notebooks e scripts, utilizando o comando:
    ```
    pip install pandas numpy torch scikit-learn matplotlib pygad
    ```

3. **Executando Notebooks:**

    Abra o VS Code e instale a extensão oficial Jupyter (Microsoft) pela barra lateral de extensões.

    Com a extensão instalada, basta clicar duas vezes no arquivo .ipynb e selecionar o kernel Python desejado.

    Execute as células na ordem para visualizar os resultados.

4. **Executando Scripts Python (.py):**

    Para scripts como xlstm_ga_search.py, que fazem otimização genética diretamente em Python (fora do notebook), utilize o terminal:
    ```
    python xlstm_ga_search.py
    ```

5. **Sobre o Script .py**

    O script pode usar bibliotecas específicas, então, além dos pacotes comuns, certifique-se de ter o pacote pygad instalado.

    O início do script deve conter os imports necessários:

    ```
    import pandas as pd
    import numpy as np
    import torch
    import torch.nn as nn
    import torch.optim as optim
    from sklearn.preprocessing import MinMaxScaler
    from torch.utils.data import TensorDataset, DataLoader
    import pygad
    ```
    Ao rodar, o script irá testar diferentes hiperparâmetros para o modelo e, ao final, exibirá no terminal a configuração ótima encontrada.

6. **Observações:**

    Os resultados podem variar ligeiramente a cada execução devido à natureza dos algoritmos evolutivos e inicialização aleatória dos modelos.

     **Importante ! (olhar o caminho do CSV)**  Certifique-se de que todos os arquivos necessários (scripts, notebooks e dataset) estejam na mesma pasta, ou ajuste os caminhos conforme necessário.

    Caso utilize o Google Colab, basta fazer upload dos arquivos e seguir os comandos nas células dos notebooks.

