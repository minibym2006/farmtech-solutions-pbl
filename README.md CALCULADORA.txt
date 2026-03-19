# 🚜 FarmTech Solutions - Inteligência Artificial e Arquitetura em Nuvem

Bem-vindo(a) ao repositório do projeto desenvolvido para a **FarmTech Solutions**. 

Este projeto engloba as Entregas 1 e 2 (Fases 4 e 5) e tem como objetivo ajudar uma fazenda de médio porte (aproximadamente 200 hectares) a analisar e prever o rendimento das suas safras, além de projetar a infraestrutura em nuvem necessária para hospedar a solução.

---

## 🌾 Entrega 1: Previsão de Rendimento de Safra (Machine Learning)

Através dos dados climáticos e agrícolas fornecidos (`crop_yield.csv`), nossa equipe desenvolveu uma solução de Inteligência Artificial contemplando:
1. **Análise Exploratória de Dados (EDA):** Compreensão das variáveis de precipitação, umidade e temperatura.
2. **Machine Learning Não Supervisionado:** Uso de K-Means e Boxplots para clusterização e identificação de anomalias (outliers) na produtividade.
3. **Machine Learning Supervisionado:** Construção e avaliação de 5 modelos preditivos (Regressão Linear, Árvore de Decisão, Random Forest, SVR e Gradient Boosting) para prever o rendimento em toneladas por hectare.

### 📂 Acesso ao Código
Todo o código, gráficos e conclusões da Entrega 1 estão documentados no nosso Jupyter Notebook.
👉 **[Clique aqui para acessar o Jupyter Notebook do projeto](SeuNome_rmXXXXX_pbl_fase4.ipynb)**

### 🎥 Demonstração em Vídeo (Machine Learning)
👉 **[Assista à demonstração da Entrega 1 no YouTube](COLOQUE_LINK_DO_VIDEO_1_AQUI)**

---

## ☁️ Entrega 2: Hospedagem e Arquitetura em Nuvem (AWS)

Para garantir que a API e o modelo de Machine Learning recebam os dados dos sensores da fazenda 24/7, projetamos a infraestrutura utilizando a **Amazon Web Services (AWS)**.

### 1. Estimativa de Custos: Virgínia do Norte vs. São Paulo
Buscamos a solução que atendesse aos requisitos: **2 vCPUs, 1 GiB de memória, até 5 Gigabit de rede e 50 GB de armazenamento**. A instância escolhida foi a **`t3.micro`** (Linux, 100% On-Demand).

| Região AWS | Instância (EC2 `t3.micro`) | Armazenamento (50 GB) | Custo Mensal Estimado |
| :--- | :--- | :--- | :--- |
| **US East (N. Virginia)** | [Preencha o valor em $] | [Preencha o valor em $] | **[Preencha o Total]** |
| **South America (São Paulo)**| [Preencha o valor em $] | [Preencha o valor em $] | **[Preencha o Total]** |

> **Evidências (AWS Pricing Calculator):**
> *(Arraste os prints da calculadora para cá)*
> `[Print N. Virginia]`
> `[Print São Paulo]`

### 2. Decisão Arquitetural
Apesar da região da Virgínia do Norte ser financeiramente mais barata, a nossa decisão de negócio é **hospedar a aplicação na região de São Paulo (BR)**. 

**Justificativa:**
* **Restrições Legais:** O projeto possui restrições explícitas que impedem o armazenamento dos dados da fazenda no exterior. O servidor no Brasil garante a conformidade com as leis locais.
* **Baixa Latência:** Precisamos acessar rapidamente os dados dos sensores. Com a fazenda localizada no Brasil, a distância até o data center em São Paulo é muito menor, permitindo respostas em tempo real da nossa Inteligência Artificial.

### 🎥 Demonstração em Vídeo (Cloud Computing)
👉 **[Assista à simulação na AWS no YouTube](COLOQUE_LINK_DO_VIDEO_2_AQUI)**

---

## 🛠️ Tecnologias Utilizadas
* **Linguagem & Bibliotecas:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn
* **Ambiente de Desenvolvimento:** Google Colab / Jupyter Notebook
* **Cloud Computing:** Amazon Web Services (AWS Pricing Calculator, EC2, EBS)

## 👥 Integrantes do Grupo
* **[Nome do Integrante 1]** - RM: [XXXXX]
* **[Nome do Integrante 2]** - RM: [XXXXX]
* **[Nome do Integrante 3]** - RM: [XXXXX]
* **[Nome do Integrante 4]** - RM: [XXXXX]
* **[Nome do Integrante 5]** - RM: [XXXXX]