# Projeto de Classificação de Imagens com CNN e Transfer Learning

Este projeto tem como objetivo desenvolver um modelo de classificação de imagens utilizando uma arquitetura de Rede Neural Convolucional (CNN) e técnicas de Transfer Learning com a rede pré-treinada VGG16. O dataset utilizado é o CIFAR-10, que contém 60.000 imagens coloridas de 10 classes diferentes.

## Estrutura do Projeto

1. **Carregamento e Visualização de Imagens**
   - Carregar o dataset CIFAR-10.
   - Visualizar algumas imagens de exemplo utilizando a biblioteca matplotlib.

2. **Pré-processamento de Imagens**
   - Redimensionar as imagens para uma resolução de 34x34 pixels.
   - Normalizar os valores dos pixels para o intervalo [0, 1].
   - Combinar os conjuntos de treinamento e teste originais e dividir em novos conjuntos de treinamento e teste.

3. **Classificação de Imagens com CNN**
   - Dividir o conjunto de dados combinado em novos conjuntos de treinamento e teste.
   - Projetar e treinar uma CNN utilizando TensorFlow/Keras.
   - Avaliar o desempenho do modelo nos dados de teste e calcular a acurácia.

4. **Transfer Learning**
   - Utilizar a rede VGG16 pré-treinada e realizar transfer learning para treinar um classificador no conjunto de dados CIFAR-10.
   - Adicionar uma nova camada de classificação ao modelo.
   - Treinar apenas os parâmetros da nova camada de classificação, mantendo os pesos das camadas pré-treinadas fixos.
   - Avaliar o desempenho do modelo nos dados de teste.

## Dependências

- TensorFlow
- Keras
- NumPy
- scikit-learn
- Pillow
- Matplotlib

## Como Executar

O projeto foi desenvolvido utilizando o Google Colab, e você pode executá-lo diretamente no Google Colab para aproveitar a infraestrutura de hardware oferecida.

1. Abra o Google Colab e faça o upload do notebook `DFCom.ipynb`.

2. Instale as dependências necessárias executando a célula abaixo no Google Colab.

```python
!pip install tensorflow keras numpy scikit-learn pillow matplotlib
