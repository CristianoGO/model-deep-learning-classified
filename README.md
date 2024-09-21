# Modelo de deep learning para classificação de imagens dermatoscópicas

## Instruções do projeto

Neste projeto, você irá desenvolver um notebook em Python onde construirá um classificador para prever se uma imagem dermatoscópica é melanoma ou carcinoma basocelular.

### Acesso a base da dados

* Acesse a base pública do ISIC Challenge Datasets em https://challenge.isic-archive.com/data/#2020
* No Training Data baixe o conjunto de imagens em Download JPEG
* No 	Training Ground Truth baixo o arquivo.csv para rotulagem das imagens
  
  #### Após baixar os arquivos necessários faça a divisão das classes e rotulagem das imagens
  * Classes:
    1. Melanoma
    2. Carcinoma basocelular
  * Na pasta 02-label_imgs do projeto existe um arquivo chamado label_imgs que ajuda a rotular as imagens
 
### Sistema operacional

* Linux Ubuntu na versão 24.04.1 LTS
 
### Linguagem de programação 

* Python 3.0

### Ambiente de desenvolvimento

* Criamos um ambiente de desenvolvimento virtual no anaconda-navigator. Baixar em https://www.anaconda.com/products/navigator
* Implementamos os códigos utiliznado o Jupyter Notebook. Baixar em https://jupyter.org/install
  * Na pasta 01-mobileNetV2 do projeto existe o arquivo modified_mobilenetv2_30 onde está o código da construção e treinamento do modelo

    #### Observações:
    1. Instale todas as bibliotecas necessárioas para o projeto
    2. Configure seu ambiente de desenvolvimento virtual
    3. Altere o caminho das pastas no codigo de acordo a estrutura do seu projeto
   
### Recursos utilizados na construção do modelo

* Transferência indutiva (Transfer learning)
* MobileNetV2
* Cross-validation

### Considerações finais

* O modelo foi treinado com 30 épocas, o que pode torna o processo de treinamento demorado, mas isso vai depender das configurações do seu computador
* Apos cada o treinamento de cada época é gerada uma matriz de confusão como na imagem abaixo:
  ![Matriz de confusão para cada fold](https://github.com/CristianoGO/model-deep-learning-classified/blob/main/coding/01-mobileNetV2/fold_30/Screenshot%20from%202024-09-21%2015-20-55.png)
