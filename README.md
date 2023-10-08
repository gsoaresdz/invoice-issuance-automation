# **Automação - Sistema de emissão de nota fiscal eletrônica NFe**

Este repositório contém um script Python de automação que emite notas fiscais eletrônicas (NFe) utilizando Selenium WebDriver e Pandas. Ele lê um arquivo Excel com informações dos clientes e preenche um formulário na página web para gerar as notas fiscais correspondentes.

## **Requisitos**

- Python 3.x
- Selenium WebDriver
- ChromeDriver
- Pandas

## **Instalação**

1. Clone o repositório:

```
git clone https://github.com/seu-usuario/seu-repositorio.git

```

1. Instale as dependências:

```
pip install selenium pandas openpyxl webdriver-manager

```

## **Uso**

1. Atualize o arquivo **`NotasEmitir.xlsx`** com as informações dos clientes e produtos/serviços para os quais você deseja emitir notas fiscais.
2. Atualize o script com suas credenciais de login e caminhos de diretório desejados.
3. Execute o script:

```
python main.py

```

Após a execução bem-sucedida, as notas fiscais serão emitidas e os arquivos baixados no diretório especificado.

## **Funcionalidades**

O script realiza as seguintes ações:

1. Configura o navegador Chrome com opções de download automático.
2. Acessa a página de login e realiza o login com as credenciais fornecidas.
3. Importa a base de clientes a partir do arquivo Excel **`NotasEmitir.xlsx`**.
4. Para cada cliente, preenche o formulário de emissão de nota fiscal com as informações correspondentes e emite a nota.
5. Encerra o navegador após a conclusão do processo.

## **Limitações**

- Este script foi projetado para funcionar com o ChromeDriver e pode não ser compatível com outros navegadores.
- Os dados de login e senha estão hardcoded no script. Recomenda-se armazená-los de forma segura em um arquivo de configuração ou variáveis de ambiente.
- O script assume que o layout do formulário e os seletores do DOM não mudarão. Se a página for atualizada, os seletores podem precisar ser ajustados.
