# **Análise Espectral de Compostos**

## **Visão Geral**
O projeto visa o desenvolvimento de um sistema de análise espectral para identificação e quantificação de elementos presentes em misturas. O sistema permite aos usuários selecionarem áreas de interesse em uma imagem e analisar a refletância espectral dessas áreas em diferentes bandas espectrais. Dessa forma, é possível verificar a proporção, classificar e categorizar os elementos da composição analisada. Além da seleção manual, o sistema também realiza a **seleção automática das áreas de interesse**, otimizando o processo de análise.

## **Objetivos**
- Identificar os elementos presentes na mistura por meio da análise espectral.
- Classificar os pixels da imagem de acordo com as características espectrais.
- Avaliar a distribuição espacial dos elementos na imagem.
- Quantificar a ocorrência de cada elemento em regiões específicas.
- Gerar gráficos detalhados da análise espectral.

## **Metodologia**

### **Aquisição e Processamento de Imagem**
- As imagens espectrais são capturadas e processadas para realce das bandas de interesse.
- O sistema permite tanto a seleção manual quanto a **seleção automática** das áreas de interesse para análise detalhada.

<div style="display: flex; flex-direction: 'row'; justify-content: center; align-items: center; gap:40px">
<img src="/images/asa.png" height="500px">

<img src="/images/auto.png" height="500px">
</div>

> *Exemplo de imagem espectral com seleção automática das áreas de interesse.*

### **Classificação por Aprendizado de Máquina**
- Utilização do modelo **SVM (Máquina de Vetores de Suporte)** para classificar os pixels da imagem.
- Os pixels são categorizados em diferentes classes, correspondentes aos elementos presentes na mistura.

<div style="display: flex; flex-direction: 'row'; justify-content: center; align-items: center; gap:40px">
<img src="/images/reflectancia.png" height="350px">
</div>

> *Gráfico ilustrando a classificação dos elementos pelo modelo SVM.*

### **Análise Espacial da Distribuição dos Elementos**
- A imagem é segmentada em **quadrantes** para avaliação da homogeneidade espacial.
- O desvio padrão da coerência espacial dentro de cada quadrante é calculado.
- **Gráficos são gerados** para representar a distribuição dos elementos.

<div style="display: flex; flex-direction: 'row'; justify-content: center; align-items: center; gap:40px">
<img src="/images/separacao.png" height="350px">
</div>

> *Distribuição espacial dos elementos com análise de coerência.*

## **Resultados**
Os testes realizados demonstraram a eficácia do sistema na **classificação e quantificação dos elementos** presentes nas misturas analisadas. Os principais resultados incluem:
- **Classificação precisa dos pixels** em diferentes categorias espectrais.
- **Identificação da proporção** de cada elemento dentro da amostra.
- **Análise da homogeneidade espacial**, auxiliando na avaliação da distribuição dos compostos.
- **Geração de gráficos detalhados** para visualização e interpretação dos dados espectrais.

<div style="display: flex; flex-direction: 'row'; justify-content: center; align-items: center; gap:20px">
<img src="/images/matriz.png" height="350px">
<img src="/images/pca.png" height="350px">
</div>

> *Gráficos representando a precisão das classificações.*

## **Tecnologias Utilizadas**
- **Linguagem:** Python
- **Bibliotecas:** OpenCV, Scikit-Learn, NumPy, Matplotlib
- **Técnicas:** Processamento de imagem, aprendizado de máquina (SVM), análise espectral, geração de gráficos


