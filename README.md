# Jogador Automático de Forca

Integrantes:
* Carlos Hernani

Este projeto implementa um jogador automático para o jogo da forca, utilizando conceitos de **entropia** e **teoria da informação** para escolher letras estrategicamente. O objetivo do jogador é adivinhar a palavra correta no menor número de tentativas, maximizando a taxa de vitórias em partidas simuladas com apenas 5 vidas.

## Descrição do Projeto

O projeto simula um jogador automático de forca usando uma lista de palavras do vocabulário da língua portuguesa. A abordagem central do projeto é a aplicação do conceito de entropia, permitindo que o jogador escolha as letras com maior potencial informativo em cada jogada. Esse método aumenta as chances de acerto, pois o jogador prioriza as letras que trazem mais informação sobre a palavra desconhecida.

O projeto está dividido em etapas principais:
1. **Carregamento do Vocabulário**: A lista de palavras é obtida a partir de uma URL fornecida e armazenada para consulta.
2. **Cálculo de Entropia**: Em cada jogada, o jogador calcula a entropia de cada letra nas palavras possíveis e escolhe a letra com maior entropia, ou seja, a letra que traz mais informação sobre a palavra.
3. **Jogada e Filtragem de Possibilidades**: Com cada jogada, o jogador atualiza as possíveis palavras, mantendo apenas aquelas que são compatíveis com as letras e posições reveladas.
4. **Simulação de Múltiplos Jogos**: A simulação executa uma série de jogos (padrão de 100 jogos) para avaliar a taxa de sucesso do jogador automático.

## Conceitos de Álgebra Linear e Teoria da Informação

O conceito central aplicado no projeto é **entropia** (informação esperada), que vem da teoria da informação. Entropia mede a quantidade de incerteza ou imprevisibilidade em uma variável. Neste caso, a entropia é usada para avaliar o quanto a escolha de uma letra pode reduzir a incerteza sobre a palavra alvo. O jogador calcula a entropia para cada letra que ainda não foi tentada e escolhe a que oferece a maior redução de incerteza.

## Arquivos do Projeto

- `demo.ipynb`: Jupyter Notebook comentado e executado, que contém o código completo e os resultados de uma simulação de 100 jogos.
- `README.md`: Este arquivo, que explica a estrutura do projeto, os conceitos aplicados e os resultados.

## Resultados da Simulação

Na simulação padrão com 100 jogos, o jogador automático apresentou o seguinte desempenho:
- **Vitórias**: 100
- **Derrotas**: 0
- **Taxa de Sucesso**: 100%
- **Taxa de Derrota**: 0%
- **Média de Tentativas em Vitórias**: 1.44 tentativas por partida vitoriosa.

### Análise de Palavras Difíceis

Nenhuma palavra específica causou dificuldades ao jogador automático, pois ele foi bem-sucedido em todas as partidas simuladas. Esse resultado demonstra a eficácia da estratégia baseada em entropia para escolher letras informativas e rapidamente restringir as possíveis palavras.

## Instruções para Execução

Para reproduzir os resultados, execute o notebook `demo.ipynb` em um ambiente Jupyter com acesso à internet (para o carregamento do vocabulário). O notebook já está executado, mas pode ser reexecutado para verificar diferentes resultados de simulação.

## Conclusão

Este projeto demonstra como a aplicação de entropia pode ser eficaz em um jogo de forca, permitindo que o jogador automático maximize suas chances de acerto com um número limitado de tentativas. Além disso, a análise das falhas e das palavras difíceis revela áreas onde a estratégia pode ser aprimorada, oferecendo direções para futuras melhorias.

