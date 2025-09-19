# pipeline_dados

Este projeto é um **pipeline de dados** construído como parte de um curso focado nos fundamentos da Engenharia de Dados.  
O objetivo é aplicar a **engenharia de software** na criação de um pipeline que cuida das etapas de **extração, transformação e carregamento (ETL)** de dados, utilizando o paradigma de **orientação a objeto**.

---

## 🎯 Descrição do Projeto

O objetivo principal deste projeto é desenvolver um **pipeline de dados reutilizável** para a fusão de duas grandes empresas.  
As empresas **A** e **B** possuem bases de dados de origens e estruturas diferentes, e a equipe de análise precisa de um **relatório consolidado** para obter insights sobre o desempenho das vendas pós-fusão.

Este pipeline terá a responsabilidade de:

- **Extrair** dados de duas fontes distintas (uma em **CSV** e outra em **JSON**).
- **Transformar** esses dados para que tenham uma estrutura unificada e consistente.
- **Carregar** os dados transformados para que a equipe de **BI/Analytics** possa gerar relatórios e obter insights.

O projeto é uma introdução à **engenharia de dados**, com foco na construção de uma solução sólida e fundamentada, **sem a utilização de ferramentas de Big Data mais complexas**.  
Ele reforça a **lógica de programação** e a aplicação de **orientação a objeto** para criar um código robusto e eficiente.

---

## 📂 Estrutura do Repositório

  pipeline_dados/
  │── data_raw/ # Pasta destinada a armazenar os dados brutos
  │── scripts/ # Contém os scripts e o código-fonte do projeto
  │── venv/ # Ambiente virtual do Python

  
---

## 🛠️ Tecnologias

- **Python** (96.3%)
- Pequenas partes em **Cython**, **C** e **C++**

---

## 💻 Ferramentas de Desenvolvimento

- **Visual Studio Code**
- **WSL (Windows Subsystem for Linux)**

### 🔹 Instalando o VS Code

1. Baixe o instalador do VS Code no [site oficial](https://code.visualstudio.com/).
2. Execute o instalador e, na tela **"Selecionar Tarefas Adicionais"**, certifique-se de marcar a opção **"Adicione em PATH"**.
3. Continue a instalação até a conclusão.

### 🔹 Configurando o VS Code com WSL

No terminal do WSL, navegue até a pasta do seu projeto:

```bash
cd pipeline_dados 
```
Abra o VS Code no diretório atual:

code .

### No VS Code:

- Vá para a seção "Extensions" (Extensões).
- Procure por "WSL" e instale a extensão.
- Feche e reabra o VS Code usando novamente:

4. Confirme se a conexão com o WSL está ativa verificando no canto inferior esquerdo a sinalização:
WSL: Ubuntu-22.04

📦 Extensões Essenciais

Python → Desenvolvimento, depuração e execução de programas Python.

Jupyter → Para trabalhar com notebooks Jupyter.

🐍 Ambiente Python e Instalação
🔹 Atualizando pacotes do sistema
sudo apt-get update
sudo apt-get upgrade -y

🔹 Verificando versão do Python
python3 --version


Se necessário, instale a versão 3.10:

sudo apt update
sudo apt install python3.10

🔹 Instalando pip e venv
sudo apt install python3-pip -y
sudo apt install python3-venv -y

🔹 Criando ambiente virtual
cd pipeline_dados
python3 -m venv venv
source venv/bin/activate

🔹 Instalando bibliotecas necessárias
pip install requests==2.28.2
pip install pandas==2.0.0

📊 Obtenção dos Dados

Para iniciar o desenvolvimento, obtenha os dados brutos com wget no terminal do WSL.

Navegue até a pasta de dados brutos:
```cd data_raw```

### Baixe os arquivos CSV e JSON:
```
-  wget https://raw.githubusercontent.com/alura-cursos/Pipeline-de-dados-combinando-Python-e-orientcao-a-objeto/main/data_raw/dados_empresaB.csv 
-  wget https://raw.githubusercontent.com/alura-cursos/Pipeline-de-dados-combinando-Python-e-orientcao-a-objeto/main/data_raw/dados_empresaA.json 
```
