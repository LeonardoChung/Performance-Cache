# **Aplicativo de Leitura de Textos com Memória Cache**

## **Descrição**

Este é um programa desenvolvido para simular um aplicativo de leitura de textos com gerenciamento de memória cache, como parte da matéria **Performance em Sistemas Ciberfísicos - PUCPR**. O aplicativo permite a leitura de textos identificados por números e realiza simulações para demonstrar o funcionamento de diferentes algoritmos de cache: **LFU (Least Frequently Used)**, **LRU (Least Recently Used)** e **FIFO (First-In First-Out)**.

## **Como Funciona**

### **Execução do Programa**

Ao iniciar o programa, você será solicitado a fornecer um número de entrada. As opções de entrada são as seguintes:

- **1 a 100**: Abre e apresenta na tela o texto identificado pelo número para leitura.
- **0**: Encerra o programa.
- **-1**: O programa entra no modo de simulação.

### **Textos**

- O programa contém 100 textos, cada um com pelo menos 1000 palavras, gerados no início do código.
- Estes textos são acessíveis pelos números de 1 a 100.

### **Modo de Simulação**

O modo de simulação realiza o seguinte:

1. **Funcionamento dos Algoritmos de Cache**: Simula o comportamento dos algoritmos LFU, LRU e FIFO.
2. **Solicitações de Usuários**: Para 200 solicitações feitas por 3 usuários diferentes, o número do texto é selecionado de três maneiras diferentes:
   - **Aleatório puro e simples**.
   - **Aleatório com distribuição de Poisson**.
   - **Aleatório com 33% de chance de selecionar textos numerados entre 30 e 40**.

3. **Relatório Gerado**: Ao final da simulação, um relatório em formato de texto é gerado contendo:
   - Estatísticas para cada usuário.
   - Desempenho de cada algoritmo de cache.
   - Tempos de apresentação de cada texto.
   - Número de ocorrências de **cache miss** (quando o texto não estava no cache) e **cache hit** (quando o texto estava no cache).
