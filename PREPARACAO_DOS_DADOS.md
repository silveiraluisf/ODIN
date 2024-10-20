[< Voltar](/README.md)

# Preparação dos Dados
  Foi utilizado como padrão para as anotações(labeling) e organização de pastas o Roboflow(https://roboflow.com/). É necessário a utilização do Google Drive ou seja seu dataset PRECISA estar dentro dele.

## Definição do caminho do dataset
  Ao inserir o caminho, o google drive já será considerado na inserção como no exemplo abaixo:
  ![image](https://user-images.githubusercontent.com/20934770/151736715-89beb853-6dd9-4737-be5c-b6199b3b7764.png)
  
  Caso não exista o diretório ou esteja com formato incorreto ele retornará os exemplos de erros abaixo:
  ![image](https://user-images.githubusercontent.com/20934770/151736983-c00f24c4-c755-40bf-a9aa-b0be7b5ca3e5.png)
  ![image](https://user-images.githubusercontent.com/20934770/151737054-e2bef490-8724-4244-9d2f-ac63c75426af.png)

## Organização das pastas
  O dataset precisa estar em um padrão definido por 3 pastas ('test', 'train' e 'valid') e 1 arquivo ('data.yaml') como na imagem a seguir:
![image](https://user-images.githubusercontent.com/20934770/151734484-4db96339-a55d-4db2-be48-418d7a6bfd90.png)

## train
  A pasta 'train' é utilizada para treinar o modelo.
### Organização
  É necessário dentro dela existir 2 pastas, uma para as imagens (images) e a outra para os labels
  ![image](https://user-images.githubusercontent.com/20934770/151734796-b38b67fb-605c-45dd-85ae-2668ab5a1226.png)

## valid
  A pasta 'valid' é utilizada para à avaliação do treinamento, podendo ter uma precisão maior de quanto seu modelo está melhorando.
### Organização
  É necessário dentro dela existir 2 pastas, uma para as imagens (images) e a outra para os labels
  ![image](https://user-images.githubusercontent.com/20934770/151734796-b38b67fb-605c-45dd-85ae-2668ab5a1226.png)

## test
  A pasta 'test' é utilizada para fazer a predição ao final do treinamento do modelo, podendo assim verificar a qualidade e a efetividade do seu conjunto de treinamento.
### Organização
  É necessário dentro dela existir 2 pastas, uma para as imagens (images) e a outra para os labels
  ![image](https://user-images.githubusercontent.com/20934770/151734796-b38b67fb-605c-45dd-85ae-2668ab5a1226.png)

## data.yaml
  É o arquivo contendo as configurações para o treinamento, como caminho da pasta 'train' e 'valid', número de classes do dataset e a lista de classes.
  
  ![image](https://user-images.githubusercontent.com/20934770/151735219-ae8fb2c7-ed3c-44b6-a84c-81380b2ea063.png)
  
  Obs: este arquivo em alguns casos se chama custom.yaml mas para utilizar a ferramenta será necessário altera-lo para data.yaml
