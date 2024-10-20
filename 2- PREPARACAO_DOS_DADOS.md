[< Voltar](/README.md)

# Preparação dos Dados
  Há duas maneiras de importar o conjunto de dados para o ODIN. A primeira é através de uma pasta no Google Drive, e a segunda é através de um Code Snippet do Roboflow. A seguir, será apresentado o tutorial para ambas opções.

## 1 - Pasta no Google Drive
  Foi utilizado como padrão para as anotações(labeling) e organização de pastas o Roboflow(https://roboflow.com/). É necessário a utilização do Google Drive ou seja seu dataset PRECISA estar dentro dele.

### Definição do caminho do dataset
  Ao inserir o caminho, o google drive já será considerado na inserção como no exemplo abaixo:
  ![Captura de tela 2024-10-20 103310](https://github.com/user-attachments/assets/1e0d2ef4-1557-41d9-9ba6-bfcb8149a119)

  Caso não exista o diretório ou esteja com formato incorreto ele retornará o exemplo de erro abaixo:
  ![Captura de tela 2024-10-20 103526](https://github.com/user-attachments/assets/a45eab0d-f122-4622-8f26-5c1d3ca07877)


### Organização das pastas
  O dataset precisa estar em um padrão definido por 3 pastas ('test', 'train' e 'valid') e 1 arquivo ('data.yaml') como na imagem a seguir:
  
![image](https://user-images.githubusercontent.com/20934770/151734484-4db96339-a55d-4db2-be48-418d7a6bfd90.png)

### train
  A pasta 'train' é utilizada para treinar o modelo.
#### Organização
  É necessário dentro dela existir 2 pastas, uma para as imagens (images) e a outra para os labels
  ![image](https://user-images.githubusercontent.com/20934770/151734796-b38b67fb-605c-45dd-85ae-2668ab5a1226.png)

### valid
  A pasta 'valid' é utilizada para à avaliação do treinamento, podendo ter uma precisão maior de quanto seu modelo está melhorando.
#### Organização
  É necessário dentro dela existir 2 pastas, uma para as imagens (images) e a outra para os labels
  ![image](https://user-images.githubusercontent.com/20934770/151734796-b38b67fb-605c-45dd-85ae-2668ab5a1226.png)

### test
  A pasta 'test' é utilizada para fazer a predição ao final do treinamento do modelo, podendo assim verificar a qualidade e a efetividade do seu conjunto de treinamento.
#### Organização
  É necessário dentro dela existir 2 pastas, uma para as imagens (images) e a outra para os labels
  ![image](https://user-images.githubusercontent.com/20934770/151734796-b38b67fb-605c-45dd-85ae-2668ab5a1226.png)

### data.yaml
  É o arquivo contendo as configurações para o treinamento, como caminho da pasta 'train' e 'valid', número de classes do dataset e a lista de classes.
  
  ![image](https://user-images.githubusercontent.com/20934770/151735219-ae8fb2c7-ed3c-44b6-a84c-81380b2ea063.png)
  
  Obs: este arquivo em alguns casos se chama custom.yaml mas para utilizar a ferramenta será necessário altera-lo para data.yaml

  ## 2- Code Snippet
  Para importar o conjunto de dados diretamente do Roboflow você deve acessar o painel "Versions" em seguida clicar no botão de "Download Dataset":
  ![Captura de tela 2024-10-20 103926](https://github.com/user-attachments/assets/8c66cefe-5a4c-45fe-8a19-df41a5471d12)

  Selecione a versão do YOLO, que deve ser ou "YOLOv5 PyTorch" ou "YOLOv8":
  ![Captura de tela 2024-10-20 104007](https://github.com/user-attachments/assets/dd95d87d-f510-42cb-8ffe-a4ea1565bd88)

  O Roboflow irá preparar o "Code Snippet" para importação do conjunto de dados, isso pode levar alguns segundos. Então, quando o "Code Snippet" aparecer, você deve copiar o código inteiro: 
  ![Captura de tela 2024-10-20 104050](https://github.com/user-attachments/assets/bbbafd24-ff3c-4ed1-a785-57ada97bc072)

  No painel do ODIN, você irá colar o "Code Snippet" conforme figura abaixo e clicar em "Carregar imagens". Se tudo deu certo, irá aparecer a mensagem de sucesso conforme figura:
  ![Captura de tela 2024-10-20 104247](https://github.com/user-attachments/assets/d8f3bd5b-fce6-4954-b31c-dc1602682215)
