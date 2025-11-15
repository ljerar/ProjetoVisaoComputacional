# Detecção de Defeitos em Frutas e Hortaliças com YOLOv8, YOLOv11 e Faster R-CNN

## Descrição do Projeto

Este projeto utiliza redes neurais YOLOv8, YOLOv11 e Faster R-CNN (FRCNN) para realizar a detecção automática de defeitos em frutas e hortaliças. O objetivo é classificar e localizar frutas boas (**fresh**) e defeituosas (**rotten**) para auxiliar em processos automatizados de inspeção de qualidade.

O pipeline inclui:
- **Preparação do dataset**: Organização e rotulação de imagens.
- **Treinamento dos modelos YOLO e FRCNN**: Configuração e execução do treinamento.
- **Avaliação dos modelos**: Comparação de métricas como precisão, revocação e mAP.
- **Visualização de resultados**: Gráficos e tabelas comparativas.

---

## Estrutura do Repositório

```plaintext
visao_computacional/
├── [af_ia_frcnn.ipynb]         # Notebook para treinamento do modelo Faster R-CNN
├── [af_ia_yolo.ipynb]          # Notebook principal do projeto YOLO
├── [README.md]                 # Documentação do projeto
├── dataset_train/              # Dataset de treino principal
│   ├── fresh_apple/
│   ├── fresh_banana/
│   ├── fresh_orange/
│   ├── rotten_apple/
│   ├── rotten_banana/
│   ├── rotten_orange/
├── dataset_train2/             # Dataset de treino adicional
│   ├── fresh_apple/
│   ├── fresh_banana/
│   ├── fresh_orange/
│   ├── rotten_apple/
│   ├── rotten_banana/
│   ├── rotten_orange/
├── dataset_val/                # Dataset de validação
│   ├── fresh_apple/
│   ├── fresh_banana/
│   ├── fresh_orange/
│   ├── rotten_apple/
│   ├── rotten_banana/
│   ├── rotten_orange/
├── runs/                       # Resultados dos treinamentos
│   ├── frcnn_training/         # Resultados do modelo FRCNN
│   ├── train_fruit_v8n/        # Resultados do YOLOv8
│   ├── train_fruit_v11n/       # Resultados do YOLOv11
```

--- 

## Download dos Datasets

Os datasets utilizados neste projeto estão disponíveis no Google Drive. Para baixá-los, siga os links abaixo:

- [Dataset de Treino Principal] (https://www.kaggle.com/datasets/zlatan599/fruitquality1)
- [Dataset de Treino Adicional] (https://www.kaggle.com/datasets/muhammad0subhan/fruit-and-vegetable-disease-healthy-vs-rotten?select=Fruit+And+Vegetable+Diseases+Dataset)
- [Dataset de Validação]

Após o download, organize os datasets conforme a estrutura abaixo:

```plaintext
visao_computacional/
├── dataset_train/
│   ├── fresh_apple/
│   ├── fresh_banana/
│   ├── fresh_orange/
│   ├── rotten_apple/
│   ├── rotten_banana/
│   ├── rotten_orange/
├── dataset_train2/
│   ├── fresh_apple/
│   ├── fresh_banana/
│   ├── fresh_orange/
│   ├── rotten_apple/
│   ├── rotten_banana/
│   ├── rotten_orange/
├── dataset_val/
│   ├── fresh_apple/
│   ├── fresh_banana/
│   ├── fresh_orange/
│   ├── rotten_apple/
│   ├── rotten_banana/
│   ├── rotten_orange/