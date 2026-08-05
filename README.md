# Projeto 02 – Tradução Automática com Mecanismo de Atenção (MS671)

Projeto desenvolvido na disciplina **Introdução ao Aprendizado de Máquina Profundo (MS671)**, da Universidade Estadual de Campinas (UNICAMP).

O objetivo foi implementar um modelo **Sequence-to-Sequence (Seq2Seq)** com mecanismo de atenção para traduzir datas em diferentes formatos para o padrão **ISO 8601 (YYYY-MM-DD)**, além de analisar o processo de aprendizado e interpretar os mapas de atenção gerados pelo modelo.

## Objetivos

- implementar um modelo Seq2Seq para tradução automática;
- aplicar o mecanismo de atenção em uma tarefa de Processamento de Linguagem Natural (NLP);
- analisar o comportamento do modelo durante o treinamento;
- interpretar mapas de atenção;
- avaliar o impacto da arquitetura da rede no desempenho do modelo.

## Ferramentas utilizadas

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab

## Metodologia

O projeto foi desenvolvido em **Python** utilizando TensorFlow/Keras.

As principais etapas incluíram:

- preparação do conjunto de dados;
- treinamento de um modelo Encoder-Decoder (Seq2Seq);
- utilização do mecanismo de atenção;
- análise das curvas de treinamento;
- interpretação dos mapas de atenção;
- comparação entre um modelo treinado localmente e um modelo pré-treinado;
- avaliação de diferentes configurações da arquitetura da rede.

## Conceitos abordados

- Deep Learning
- Processamento de Linguagem Natural (NLP)
- Sequence-to-Sequence (Seq2Seq)
- Encoder-Decoder
- Mecanismo de Atenção (Attention)
- Redes Neurais Recorrentes (RNN/LSTM)
- Tradução Automática
- Mapas de Atenção

## Resultados

Os experimentos mostraram que:

- o modelo alcançou aproximadamente **80% de acurácia** após 50 épocas de treinamento;
- o mecanismo de atenção aprendeu a focar corretamente nas partes relevantes da entrada para gerar cada elemento da saída;
- a análise dos mapas de atenção tornou possível interpretar o comportamento do modelo durante a tradução;
- arquiteturas muito pequenas apresentaram underfitting, enquanto arquiteturas muito grandes aumentaram o custo computacional sem ganhos proporcionais de desempenho;
- uma configuração intermediária da rede apresentou o melhor equilíbrio entre desempenho e tempo de treinamento.

Também foi realizada uma comparação entre o modelo treinado localmente e um modelo pré-treinado, discutindo diferenças de desempenho e possíveis causas relacionadas ao treinamento e ao conjunto de dados.

