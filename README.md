
# AutoTri - GMCAT
Triagem Automatizada de Processos de Manutenção Cadastral e Auditorias Tributárias

## - [Distribuição (Executáveis)](https://drive.google.com/drive/folders/1vXxPCR9K_Ow2ADIvdMVsAwrsgmXjRu5z?usp=sharing)
## - [Documentação](https://drive.google.com/drive/folders/1eS0YmXbdpFn6Romy1wwn3tWkGPOoeIZu?usp=sharing)

## Pré-requisitos
- [**Python 3.11.9 ou superior**](https://www.python.org/downloads/release/python-3119/)
- [**Google Chrome**](https://www.google.com/intl/pt-BR/chrome/)  - Navegador obrigatório utilizado pelo WebDriver (Selenium)

## Como Desenvolver - PowerShell (Windows)

Clonar e acessar o repositório:
```powershell
git clone https://github.com/GMCAT4B/AutoTri-GMCAT.git
cd AutoTri-GMCAT

```

Criar e ativar ambiente virtual (Windows):

```powershell
python -m venv venv
.\venv\Scripts\activate

```

Instalar dependências:

```powershell
pip install -r requirements.txt

```

Rodar ou testar a aplicação (Interpretador / Modo Dev):

```powershell
python app\main.py

```

## Build (Gerar Executável)

Gerar executável via PyInstaller:

```powershell
pyinstaller --noconfirm --onefile --windowed --name "AutoTriagem-PBH 1_63a" --icon "app/assets/PBH-Iconizado.ico" --paths "app" --add-data "app/assets/PBH-Iconizado.ico;assets" --clean app/main.py
```
**\* Substitua o name pelo nome do executável que vais gerar com o comando do pyinstaller. Por exemplo: se quiser gerar um app com nome "AutoTriagem-PBH X_YZβ" (para versão X.YZβ) use:**

--name "AutoTriagem-PBH X_YZβ"

## Dados Locais e Persistência

Armazenamento de configurações persistentes entre execuções:

* **Caminho:** `%APPDATA%/AutoTri/`

