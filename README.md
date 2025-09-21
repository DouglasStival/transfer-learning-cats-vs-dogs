# Transfer Learning: Cats vs Dogs

## Descrição
Projeto que aplica Transfer Learning (MobileNetV2) para classificar imagens de gatos e cachorros. Implementado em Python (TensorFlow/Keras) no Google Colab.

## Estrutura do repositório
- `transfer_learning_cats_vs_dogs.ipynb` : Notebook com o código passo a passo.
- `images/` : Gráficos e exemplos de previsões.
- `requirements.txt` : Dependências.
- `final_model.zip` : (opcional) modelo salvo.

## Dataset
- Fonte: `cats_and_dogs_filtered` (Google).
- Pré-processamento: redimensionamento para 224x224, normalização via `preprocess_input`, data augmentation (flip, rotação, zoom).

## Modelo
- Base: MobileNetV2 (pretrained on ImageNet), `include_top=False`.
- Cabeça: GlobalAveragePooling2D → Dropout(0.3) → Dense(1, sigmoid).
- Treinamento: fase 1 (base congelada), fase 2 (fine-tuning das camadas finais).

## Como executar
1. Abra `transfer_learning_cats_vs_dogs.ipynb` no Google Colab.
2. Em Runtime → Change runtime type → GPU.
3. Execute as células na ordem (célula 1 → célula 8).
4. Para reproduzir, rode todas as células e baixe os artefatos via Files → Download.

## Resultados (preencher com seus números)
- Acurácia final (val): __________
- Observações: __________

## Contato
Seu Nome — seu.email@example.com
