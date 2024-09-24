# Criação de um database e Treinamento de uma rede de classificação YOLO
1. Para a criação do database, baixei algumas imagens de gatos e cachorros, sendo inicialmente 24 de cada classe para treinamento e 8 de cada classe para validação. Além de ter 26 imagens de cada classe para teste.
2. No site [MakeSense.ai](https://www.makesense.ai/) eu fiz a segmentação das imagens de treinamento e de validação e salvei em um formato yolo, o que gera as labels das imagens.
3. Devido a isso, existem 2 pastas principais, a data_test e a data_train. A data_train possui as pastas images, que contém as imagens tanto de validação quanto de treinamento, que estão separadas nas pastas train e val. A data_test possui as imagens das quais quero fazer a classificação.
4. Após o conjunto de dados de treinamento e teste, instalei uma rede YOLO ([yolov5 GitHub](https://github.com/ultralytics/yolov5)) em um notebook do [Google Colab](https://colab.research.google.com/), e fiz o treinamento e o teste das imagens.
5. O resultado não é perfeito devido a quantidade de imagens usadas para treinamento. As imagens classificadas podem ser encontradas na pasta yolov5/runs/detect/exp2.

Vale ressaltar que este é um projeto de conclusão do módulo de Redes de Deep Learning da formação [Machine Learning Specialist](https://web.dio.me/track/formacao-machine-learning-specialist) da [DIO.me](https://web.dio.me/home) e possui apenas a intenção de aprendizagem da rede de classificação yolov5.
