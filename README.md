# 🧠 Detecção de Tumores Cerebrais utilizando Inteligência Artificial

## 📌 Sobre o projeto

Este projeto tem como objetivo desenvolver e treinar um modelo de Inteligência Artificial capaz de identificar diferentes tipos de tumores cerebrais por meio da análise de imagens, utilizando o algoritmo **YOLOv8**, desenvolvido pela Ultralytics.

A solução utiliza técnicas de Deep Learning e Visão Computacional para trabalhar com imagens de ressonância magnética cerebral, buscando reconhecer quatro categorias:

- **Glioma:** tumor que se origina nas células da glia.
- **Meningioma:** tumor originado nas meninges.
- **No Tumor:** imagens sem identificação de tumor.
- **Pituitary:** tumor relacionado à hipófise.

## 🚀 Tecnologias utilizadas

- Python
- Google Colab
- YOLOv8 (Ultralytics)
- PyYAML
- Deep Learning
- Visão Computacional

## 📂 Estrutura do projeto

O projeto utiliza um dataset organizado em três conjuntos:

```text
mini_split/
├── train/
├── val/
├── test/
└── data.yaml
```

- `train`: conjunto de treinamento do modelo.
- `val`: conjunto de validação.
- `test`: conjunto de teste.
- `data.yaml`: arquivo de configuração com o caminho do dataset e as classes utilizadas.

## ⚙️ Configurações do treinamento

O modelo utilizado é o YOLOv8 Nano (`yolov8n.pt`), com os seguintes parâmetros:

| Parâmetro | Configuração |
|---|---|
| Modelo | YOLOv8 Nano |
| Épocas | 100 |
| Tamanho da imagem | 640 |
| Batch size | 16 |
| Patience | 15 |
| Pesos pré-treinados | Ativados |
| Validação | Ativada |

O treinamento é realizado utilizando a biblioteca Ultralytics.

## ▶️ Como executar o projeto

1. Faça o download ou clone este repositório.
2. Abra o arquivo `ProjetoIA.ipynb` no Google Colab.
3. Conecte sua conta do Google Drive.
4. Disponibilize o dataset na pasta `mini_split` dentro do Google Drive.
5. Confira se a estrutura do dataset está correta.
6. Execute as células do notebook na ordem apresentada.
7. Aguarde a instalação das dependências e a execução do treinamento.

**Instalação das bibliotecas:**

```bash
pip install ultralytics
pip install pyyaml
```

## 📊 Objetivo

O projeto busca explorar a aplicação de Inteligência Artificial na área da saúde, utilizando técnicas de Deep Learning e Visão Computacional para o reconhecimento de padrões em imagens cerebrais.

A proposta é estudar o treinamento de modelos capazes de auxiliar na identificação de diferentes categorias de alterações cerebrais por meio de imagens.

**Importante:** este projeto possui finalidade acadêmica e experimental. Não substitui exames, avaliação médica ou diagnóstico realizado por profissionais de saúde.

## 👨‍💻 Autor

**Jose Vitor Tavares Santiago**

Estudante de tecnologia e entusiasta de Inteligência Artificial, programação e desenvolvimento de soluções computacionais.

---

⭐ Se este projeto despertou seu interesse, fique à vontade para explorar o código e acompanhar seu desenvolvimento!
