
# SAR-Target-Detection-MLP

Desenvolvimento de um sistema para a detecção de alvos terrestres em imagens de Radar de Abertura Sintética (SAR) utilizando o dataset **CARABAS-II**. O projeto foca na implementação de Redes Neurais de Múltiplas Camadas (MLP) otimizadas por técnicas avançadas de Processamento Digital de Imagens (PDI) para filtragem de ruído e realce de alvos em cenários de vegetação densa.

## 🛠️ Tecnologias e Ferramentas

* **Linguagem:** Python
* **Processamento de Imagens:** OpenCV
* **Análise de Dados:** NumPy
* **Visualização:** Matplotlib
* **Dataset:** CARABAS-II (VHF SAR)

## 📡 Sobre o Dataset

O sensor CARABAS-II opera na banda VHF (20–90 MHz), o que permite a detecção de unidades terrestres camufladas sob copas de árvores. O principal desafio técnico reside na mitigação do ruído de *clutter* e *speckle* inerentes a sistemas de radar de baixa frequência.

## 📂 Estrutura do Projeto

* `.gitignore`: Configuração para ignorar arquivos temporários e binários pesados.
* `LICENSE`: Licença GNU GPLv3 para proteção de autoria e código aberto acadêmico.
* `carabas_images_reading.py`: Script exemplo para gerenciamento de diretórios e carregamento de imagens do CARABAS-II
* `caravas_images_process.py`: Script exemplo para processamento do dataset original e técnicas de processamento digital de imagens.

## 🚀 Metodologia

O pipeline de desenvolvimento está dividido nas seguintes etapas técnicas:

1. **Gerenciamento de Dados:** Verificação automatizada de diretórios e carregamento íntegro dos sinais de radar.
2. **Processamento Digital de Imagens (PDI):** Aplicação de filtros para redução de ruído e realce de assinaturas eletromagnéticas de alvos metálicos.
3. **Classificação via MLP:** Arquitetura de Redes Neurais de múltiplas camadas para identificação e contagem de unidades terrestres.

## 💻 Como Executar no Google Colab

Para integrar este código com o repositório de dados, utilize o seguinte fluxo no seu ambiente Colab:

```python
# Clonagem do repositório de dados
!git clone https://github.com/steinbukken7321/CARABAS-II-SAR-Dataset-Mirror.git

# Execução do script de leitura
from carabas_images_reading_exemple import manage_and_load_carabas_data

PATH_TO_DATA = "CARABAS-II-SAR-Dataset-Mirror/img"
images = manage_and_load_carabas_data(PATH_TO_DATA)

```
