# RFE-Preditor

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Online-success)](https://mas-rodrigues.github.io/RFE-Preditor/)
[![Quarto](https://img.shields.io/badge/Made%20with-Quarto-blue)](https://quarto.org)
[![R](https://img.shields.io/badge/R-276DC3?logo=r&logoColor=white)](https://www.r-project.org/)

## 📊 Sobre o Projeto

Análise estatística investigando a **espessura do músculo Reto Femoral (RFE)** como preditor da capacidade funcional em pacientes sob reabilitação cardiopulmonar. Este estudo utiliza modelos de regressão linear para identificar os principais determinantes da performance motora, mensurada pela distância de marcha.

## 🎯 Objetivo

Avaliar a relação entre morfometria muscular, percepção de sintomas e capacidade funcional, com foco em determinar se a espessura do reto femoral pode ser utilizada como biomarcador fidedigno para guiar estratégias de reabilitação fisioterapêutica.

## 🔬 Metodologia

### Coleta de Dados
- **Avaliação Morfométrica**: Ultrassonografia do músculo Reto Femoral em repouso
- **Qualidade de Vida**: Minnesota Living with Heart Failure Questionnaire (MLHFQ)
- **Capacidade Funcional**: Distância percorrida em metros (MARCHA)
- **Monitorização Hemodinâmica**: FC e SpO₂ em repouso e pós-esforço

### Análise Estatística
- Modelos de regressão linear múltipla e simples
- Matriz de correlação para identificação de relações entre variáveis
- Teste de significância com α = 0,05

## 📈 Principais Resultados

- **R²ₐⱼᵤₛₜₐ𝒹ₒ = 0,45** (p < 0,01)
- **Preditor significativo**: Espessura do Reto Femoral (p = 0,009)
- **Magnitude do efeito**: β = 221,59 (±22 metros de ganho na marcha para cada 0,1 cm de aumento no RFE)
- **Preditores não significativos**: Minnesota (p = 0,67), SpO₂ final (p = 0,23)

### Implicação Clínica

A limitação funcional demonstrou origem **periférica (muscular)** em vez de puramente ventilatória ou baseada na percepção de sintomas, reforçando a necessidade de priorizar **treinamento de força e hipertrofia de membros inferiores** na reabilitação.

## 🛠️ Tecnologias Utilizadas

- **Quarto**: Framework para publicação científica reproduzível
- **R**: Análise estatística e visualização de dados
  - `tidyverse`: Manipulação e visualização
  - `tidymodels`: Modelagem estatística
  - `googlesheets4`: Integração com Google Sheets
  - `DT`: Tabelas interativas
  - `corrr`: Análise de correlação

## 🚀 Como Visualizar

### Online (GitHub Pages)
Acesse a versão publicada: **[https://mas-rodrigues.github.io/RFE-Preditor/](https://mas-rodrigues.github.io/RFE-Preditor/)**

### Localmente

1. **Clone o repositório:**
```bash
git clone https://github.com/Mas-Rodrigues/RFE-Preditor.git
cd RFE-Preditor
```

2. **Instale as dependências do R:**
```r
install.packages(c("tidyverse", "tidymodels", "googlesheets4", "DT", "corrr", "dotenv"))
```

3. **Configure as credenciais:**
   - Crie um arquivo `.env` com suas credenciais do Google Sheets
   - Formato:
   ```
   SHEET_URL=https://docs.google.com/spreadsheets/d/SEU_ID/edit
   EMAIL=seu-email@gmail.com
   ```

4. **Renderize o documento:**
```bash
quarto render index.qmd
```

Ou visualize com live preview:
```bash
quarto preview index.qmd
```

## 📁 Estrutura do Projeto

```
RFE-Preditor/
├── index.qmd              # Documento principal Quarto
├── index.html             # Versão HTML renderizada
├── index_files/           # Recursos gerados (gráficos, libs)
│   ├── figure-html/      # Gráficos em PNG
│   └── libs/             # Bibliotecas CSS/JS
├── .env                   # Credenciais (não versionado)
├── .gitignore            # Arquivos ignorados pelo Git
└── README.md             # Este arquivo
```

## ⚠️ Limitações do Estudo

- **Tamanho amostral**: n = 12 (poder estatístico reduzido)
- **Natureza observacional**: Estabelece associação, não causalidade
- **Variabilidade individual**: Comorbidades e atividade física prévia não controladas

## 👨‍⚕️ Autor

**Marco Rodrigues**
  
🔗 GitHub: [@Mas-Rodrigues](https://github.com/Mas-Rodrigues)

## 📄 Licença

Este projeto está disponível para fins educacionais e de pesquisa.

---

⭐ **Se este projeto foi útil para você, considere deixar uma estrela no repositório!**
