# Jogador Automático de Forca

Integrantes:
- Carlos Hernani

Este projeto implementa um jogador automático para o jogo da forca, utilizando **entropia** e **teoria da informação** para escolhas estratégicas de letras. O objetivo é adivinhar a palavra correta no menor número de tentativas, maximizando a taxa de vitórias em partidas simuladas com apenas 5 vidas.

## Descrição do Projeto

O jogador automático de forca simula partidas com uma lista de palavras da língua portuguesa. O conceito central é a aplicação de entropia, permitindo ao jogador escolher as letras que trazem mais informação sobre a palavra desconhecida, aumentando assim as chances de acerto.

Principais etapas do projeto:
1. **Carregamento do Vocabulário**: A lista de palavras é carregada a partir de uma URL.
2. **Cálculo de Entropia**: Em cada jogada, o jogador calcula a entropia de cada letra e escolhe a que possui maior potencial informativo.
3. **Atualização das Possibilidades**: Após cada jogada, o jogador filtra as palavras possíveis com base nas letras reveladas.
4. **Simulação de Múltiplos Jogos**: O desempenho é avaliado em 100 jogos para medir a taxa de sucesso.

## Resultados da Simulação

Na simulação padrão de 100 jogos, o jogador automático apresentou:
- **Vitórias**: 100
- **Derrotas**: 0
- **Taxa de Sucesso**: 100%
- **Média de Tentativas**: 1.44 por vitória

Nenhuma palavra apresentou dificuldades específicas, destacando a eficácia da estratégia baseada em entropia para reduzir a incerteza e aumentar as chances de vitória.

## Instruções para Execução

Execute o notebook `demo.ipynb` em um ambiente Jupyter com acesso à internet para carregar o vocabulário. O notebook já está executado, mas pode ser reexecutado para resultados adicionais.

## Conclusão

A aplicação de entropia no jogo da forca permite ao jogador automático maximizar suas chances de acerto com tentativas limitadas. A análise das partidas bem-sucedidas demonstra a eficácia desta abordagem e sugere direções para aprimoramento contínuo.
