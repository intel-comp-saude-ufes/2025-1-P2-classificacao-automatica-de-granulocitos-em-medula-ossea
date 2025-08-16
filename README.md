# Abordagens de Aprendizado Profundo para Classificação Automatizada de Granulócitos em Medula Óssea 🩸

Este repositório contém a implementação de um projeto voltado à classificação de granulócitos utilizando Redes Neurais Convolucionais a partir de imagens de esfregaço de medula óssea. Fora aplicadas três aboradgens, sendo elas:
 - **CNN customizada** - arquitetura construída do zero, treinada inteiramente com o dataset.
 - **CNN pré-treinada com camada convolucional congelada** - utiliza uma rede previamente treinada.
 - **CNN pré-treinada com fine-tuning** - rede pré-treinada, cujas camadas convolucionais são parcialmente atualizadas durante o treinamento.

Este projeto foi desenvolvido no âmbito da disciplina de Inteligência Computacional em Saúde, ministrada pelo professor [Andre Pacheco](https://github.com/paaatcha). 

## Sumário
 - [Base de dados](#base-de-dados)
 - [Instruções de uso](#instruções-de-uso)
   - [Repositório e Dados](#repositório-e-dados)
   - [Ambiente Virtual](#ambiente-virtual)
   - [Dependências](#dependências)
   - [Execução](#execução)
 - [Notas](#notas)
 - [Contribuidores](#contribuidores)

## Base de dados
Os dados utilizados neste projeto foram obtidos do The Cancer Imaging Archive (TCIA), um repositório público de imagens médicas de câncer totalmente desidentificadas. O TCIA é financiado pelo Cancer Imaging Program (CIP), parte do National Cancer Institute (NCI, EUA), e gerenciado pelo Frederick National Laboratory for Cancer Research (FNLCR).

Para download dos arquivos, é necessário usar o IBM Aspera, uma ferramenta que permite transferir grandes volumes de dados de forma rápida e segura.

As imagens do dataset já vêm pré-processadas em 250x250 pixels, no formato JPG, e organizadas em pastas de acordo com o tipo celular. O dataset completo contém cerca de 170 mil imagens de diferentes tipos de células da medula óssea. Para este trabalho, utilizamos apenas os granulócitos, totalizando aproximadamente 80 mil imagens.

Os **dados** podem ser encontrados [aqui](https://www.cancerimagingarchive.net/collection/bone-marrow-cytomorphology_mll_helmholtz_fraunhofer/).

## Instruções de uso
Por se tratarem de arquivos `.ipynb`, podem ser executados em diversos ambientes. Todavia, recomendamos fortemente a utilização do [JupyterLab](https://jupyter.org/install) ou da [extensão](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) do Jupyter para VSCode.

### Repositório e Dados
Faça o *download* do projeto:
```bash
git clone https://github.com/intel-comp-saude-ufes/2025-1-P2-classificacao-automatica-de-granulocitos-em-medula-ossea.git && cd 2025-1-P2-classificacao-automatica-de-granulocitos-em-medula-ossea
```
 - Insira o dataset em ...

### Ambiente virtual
Crie um ambiente virtual para isolar as dependências do projeto.
```bash
python3 -m venv venv
```
```bash
source venv/bin/activate
```

### Dependências
Instale as dependências.
```bash
pip install -r requirements.txt
```
Caso opte pela utilização do JupyterLab:
```bash
pip install jupyterlab
```

### Execução
Se estiver usando a extensão do Jupyter para VSCode, basta abrir os arquivos e clicar em `Run All`. Caso esteja no JupyterLab, execute:
```bash
jupyter lab
```
e siga o mesmo procedimento.

## Notas
 - Para uma visão mais completa sobre o projeto, confira o [artigo]().
 - Confira também a apresentação em [vídeo]().
 - Os detalhes de implementação estão documentados no código.

## Contribuidores
 - [João Paulo Moura Clevelares](https://github.com/vortex2jm)
 - [Vinícius Cole de Amorim](https://github.com/viniciuscole)
 - [Thamya Vieira Hashimoto Donadia](https://github.com/thamyadonadia?tab=repositories)
