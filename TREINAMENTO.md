[< Voltar](/README.md)

## Seleção de versão
O ODIN permite que você treine seu modelo escolhendo entre as versões YOLOv5 e YOLOv8. A sua escolha deve ser feita com base na versão em que os dados foram importados.
Esta aba também permite que você exclua o modelo treinado, caso deseje fazer um novo treinamento dentro da mesma sessão do Google Colab. 

![Captura de tela 2024-10-20 111055](https://github.com/user-attachments/assets/0651e6a0-fe0e-4898-bb2b-145e6821ec7f)

## Seleção de modelo 
Após escolher a versão do YOLO, você também pode definir o modelo.

### YOLOv5
Modelos maiores como YOLOv5x e YOLOv5x6 produzirão melhores resultados em quase todos os casos, mas possuem mais parâmetros, requerem mais memória CUDA para treinar e são mais lentos para executar. Para implantações móveis, recomendamos YOLOv5n, YOLOv5s ou YOLOv5m, para implantações em nuvem, recomendamos YOLOv5l ou YOLOv5x.

![image](https://user-images.githubusercontent.com/20934770/153324590-56bf01c8-88ee-49a8-b09a-750f8bc1e46f.png)

### YOLOv8
A mesma ideia se aplicar para os modelos YOLOv8. Para implantações móveis, recomendamos YOLOv8n, YOLOv8s ou YOLOv8m, para implantações em nuvem, recomendamos YOLOv8l ou YOLOv8x. Abaixo temos um gráfico comparativo da diferença de desempenho entre as versões do YOLO.

![Captura de tela 2024-10-20 112444](https://github.com/user-attachments/assets/f81d48d8-192b-42c7-8b9e-5396241ff213)
