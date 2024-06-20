# Autores:
- Ana Luiza Martins
- Itamar Ribeiro
- Gabriella Gonçalves


# Resolvedor de Problemas de Programação Linear (PPL)

Este é um aplicativo desenvolvido em Python usando Streamlit e PuLP para resolver problemas de programação linear (PPL) utilizando o método Simplex. O aplicativo permite a entrada de dados da função objetivo e das restrições, resolve o problema e exibe os resultados, incluindo a solução ótima e os preços sombra das restrições.

## Funcionalidades

- Entrada de dados amigável para os coeficientes da função objetivo e das restrições.
- Resolução de problemas de programação linear com 2 a 4 variáveis.
- Exibição da solução ótima, valor ótimo da função objetivo e preços sombra das restrições.

## Requisitos

Certifique-se de ter o Python instalado em sua máquina. Este projeto foi testado com Python 3.9, mas versões posteriores do Python 3 também devem funcionar.

## Instalação

1. Clone este repositório ou faça o download dos arquivos.

2. Instale as bibliotecas necessárias usando pip:
    ```bash
    pip install streamlit pulp
    ```

## Como Rodar

1. Navegue até o diretório onde o arquivo `app.py` está localizado.

2. Execute o comando abaixo para iniciar o aplicativo Streamlit:
    ```bash
    streamlit run app.py
    ```

3. O navegador padrão será aberto automaticamente com a interface do aplicativo.

## Uso

1. **Função Objetivo:**
   - Insira o número de variáveis (entre 2 e 4).
   - Insira os coeficientes da função objetivo para cada variável.

2. **Restrições:**
   - Insira o número de restrições.
   - Para cada restrição, insira os coeficientes das variáveis e o limite da restrição.

3. **Resultados:**
   - A solução ótima, valor ótimo da função objetivo e preços sombra das restrições serão exibidos.

## Exemplo

Suponha que você tenha a seguinte função objetivo e restrições:

### Função Objetivo:
Maximizar \( Z = 3x_1 + 2x_2 \)

### Restrições:
1. \( x_1 + x_2 \leq 4 \)
2. \( x_1 \leq 2 \)
3. \( x_2 \leq 3 \)

Preencha os campos da seguinte forma:

1. **Função Objetivo:**
   - Número de variáveis: 2
   - Coeficiente de \( x_1 \): 3
   - Coeficiente de \( x_2 \): 2

2. **Restrições:**
   - Número de restrições: 3

   **Restrição 1:**
   - Coeficiente de \( x_1 \): 1
   - Coeficiente de \( x_2 \): 1
   - Limite da restrição: 4

   **Restrição 2:**
   - Coeficiente de \( x_1 \): 1
   - Coeficiente de \( x_2 \): 0
   - Limite da restrição: 2

   **Restrição 3:**
   - Coeficiente de \( x_1 \): 0
   - Coeficiente de \( x_2 \): 1
   - Limite da restrição: 3