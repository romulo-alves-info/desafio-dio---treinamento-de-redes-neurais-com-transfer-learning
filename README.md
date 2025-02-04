# Classificação de Imagens com Redes Neurais Convolucionais (CNN)

Este projeto implementa uma solução de classificação de imagens utilizando Redes Neurais Convolucionais (CNN) em Keras/TensorFlow. O objetivo é carregar um conjunto de imagens, processá-las, treinar um modelo CNN e avaliar o desempenho do modelo em um conjunto de dados de teste.

## Sumário
- [Instalação](#instalação)
- [Como Usar](#como-usar)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Dependências](#dependências)
- [Licença](#licença)

## Instalação

Siga os passos abaixo para configurar o ambiente e executar o código:

### 1. Clone o repositório

```bash
git clone https://github.com/romulo-alves-info/desafio-dio---treinamento-de-redes-neurais-com-transfer-learning.git
cd desafio-dio---treinamento-de-redes-neurais-com-transfer-learning
```
### 2. Instale as dependências

Se você estiver utilizando o Google Colab, você já terá a maioria das dependências instaladas por padrão. Caso esteja utilizando localmente, você pode instalar as dependências necessárias com o seguinte comando:

```bash
pip install -r requirements.txt
```

Se você não tiver o arquivo requirements.txt, basta instalar as principais dependências:

```bash
pip install tensorflow keras matplotlib pillow
```

## Como Usar

### 1. Carregar e Preparar os Dados:

- O código assume que o dataset está organizado em pastas, onde cada pasta representa uma categoria, contendo imagens dessa categoria.

- O código é projetado para funcionar com imagens em formato JPG, PNG ou JPEG. Arquivos que não sejam dessas extensões são removidos automaticamente.

### 2. Treinamento do Modelo:

- O modelo é treinado utilizando uma Rede Neural Convolucional (CNN) com camadas de convolução, pooling, dropout e densas. O treinamento usa EarlyStopping para evitar overfitting.

- O treinamento é feito usando o conjunto de dados de treino, e o modelo é validado durante o treinamento com um conjunto de dados de validação.

### 3. Exibição dos Gráficos:

- Após o treinamento, gráficos de perda e acurácia do modelo durante o treinamento são gerados para avaliação.

### 4. Avaliação do Modelo:

- O modelo treinado é avaliado em um conjunto de dados de teste, e o código exibe a perda e a acurácia do modelo para este conjunto.

## Exemplos de uso

Após configurar o ambiente e carregar o dataset, basta executar as células no notebook. O código seguirá os seguintes passos:

- Carregar as imagens.
- Criar o modelo CNN.
- Treinar o modelo.
- Exibir os gráficos de desempenho.
- Avaliar o modelo no conjunto de teste.

O código é implementado em Python, utilizando a biblioteca Keras com TensorFlow como backend.

```markdown
## Estrutura do Projeto

A estrutura básica do repositório é a seguinte:

- `/NomeDoRepositorio`
  - `/PetImages`                # Diretório com as imagens para treinamento
  - `main.py`                   # Script principal para treinamento e avaliação do modelo
  - `requirements.txt`          # Dependências do projeto
  - `README.md`                 # Este arquivo
  - `/notebooks`                # Jupyter Notebooks com exemplos e análise
```

## Dependências

Este projeto depende das seguintes bibliotecas:

- tensorflow ou keras (com backend TensorFlow)
- matplotlib (para visualização dos gráficos)
- pillow (para manipulação de imagens)
- numpy (para manipulação de dados numéricos)
- os (para manipulação de arquivos e diretórios)
- random (para embaralhar os dados)

Você pode instalar todas as dependências executando:

```bash
pip install -r requirements.txt
```

## Licença

Este projeto está licenciado sob a Licença MIT - consulte o arquivo LICENSE para mais detalhes.

Nota: Este código foi projetado para ser executado em um ambiente como o Google Colab ou uma máquina local com Python configurado corretamente.
