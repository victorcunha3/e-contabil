# e-contabil
# 🧾 Automação Fiscal - Nota Teresina (E-Contábil)

Bot desenvolvido em Python com Selenium para automação do processo de extração de documentos fiscais (XMLs e Livros Fiscais) no portal da Prefeitura de Teresina. O sistema resolve captchas automaticamente, iterando sobre múltiplas empresas e organizando os arquivos baixados por competência, otimizando a rotina de processamento de dados do escritório de contabilidade.

## 🚀 Funcionalidades

* **Login Automatizado:** Acesso dinâmico ao portal usando credenciais salvas localmente (`config_empresas.json`).
* **Bypass de Captcha:** Integração com a API do Anti-Captcha para resolução contínua via workers remotos.
* **Extração de XMLs:** Download automático das Notas Fiscais Emitidas e Recebidas de acordo com a competência informada.
* **Livros Fiscais:** Geração e download em PDF dos Livros Fiscais de Serviços Prestados e Tomados, marcando automaticamente a situação como "Normal".
* **Organização de Diretórios:** Os arquivos são dinamicamente renomeados e separados em pastas estruturadas no formato `Ano > Mês > Empresa`.

## 🛠️ Tecnologias Utilizadas

* **Python**
* **Selenium & WebDriver Manager** (Web Scraping e Automação de Navegador)
* **Anti-Captcha API** (Resolução de reCAPTCHA v2 Proxyless)
* **Dotenv** (Gerenciamento seguro de variáveis de ambiente)
