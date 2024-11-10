# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Administração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Sistema de Sensoriamento Agrícola - FarmTech Solutions

## Integrantes: 
- <a href="https://www.linkedin.com/in/joseandrefilho">Jose Andre Filho</a>

## Professores:
### Tutor 
- <a href="https://www.linkedin.com/in/lucas-gomes-moreira-15a8452a/">Lucas Gomes Moreira</a>
### Coordenador
- <a href="https://www.linkedin.com/in/profandregodoi/">André Godoi Chiovato</a>


## Descrição

O projeto **FarmTech Solutions** foi desenvolvido com o objetivo de implementar um sistema de sensoriamento agrícola, que utiliza dados de sensores de umidade, pH e nutrientes para otimizar a irrigação e a aplicação de fertilizantes nas plantações. O sistema centraliza as informações em um banco de dados, permitindo que o produtor acompanhe, em tempo real, as condições do solo e das culturas, além de prever necessidades futuras com base nos dados históricos.

O sistema foi construído com foco na gestão de dados agrícolas, abrangendo funcionalidades como:
- **Coleta de dados dos sensores**: Armazenamento e monitoramento contínuo de leituras de sensores posicionados no campo.
- **Gestão de culturas**: Cadastro e acompanhamento das plantações e suas respectivas necessidades de água e nutrientes.
- **Previsão de necessidades**: Com base nos dados históricos, o sistema prevê futuras necessidades de irrigação e aplicação de fertilizantes, utilizando técnicas de regressão linear.
- **Geração de alertas**: Notificações são geradas quando os níveis de umidade, pH ou nutrientes se encontram fora dos intervalos ideais.


## Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- **assets**: Contém imagens e outros arquivos de mídia não estruturados relacionados ao projeto.
- **mer**: Diretório que contém o arquivo do Modelo Entidade Relacionamento (MER), Diagrama Entidade Relacionamento (DER), arquivo de Definição de Dados (DDL), gerados pela ferramenta **Oracle SQL Developer Data Modeler** e o README com a documentação do Modelo de Dados.
- **src**: Diretório que contém o código fonte do projeto, arquivos de configuração e demais recursos necessários para a execução do sistema.
- **wokwi**: Diretório que contém o código fonte do projeto do Wokwi para simulação e o README com a documentação do circuito.
- **README.md**: Arquivo de guia e explicação geral sobre o projeto (este que você está lendo agora).

## Como executar o projeto
Para executar o projeto de forma completa e integrada, é importante configurar corretamente o ambiente e as dependências necessárias. Este guia irá orientá-lo em cada etapa para garantir o funcionamento ideal, desde a configuração do banco de dados até a execução local e a simulação no Wokwi. Certifique-se de seguir os passos abaixo para realizar a instalação e configurar todos os recursos que o sistema precisa.

Abaixo estão as etapas detalhadas para preparar e executar o projeto:
### Configurações necessárias:

1. **Banco de dados**:

   Para criação das tabelas necessárias para o sistema, siga as instruções do [Readme](mer/README.md)  dentro da pasta `mer`.

2. **Configurar variáveis de ambiente**:

   Crie um arquivo `.env` na raiz do projeto com as informações de acesso ao banco de dados:

   ```bash
   DB_USER=seu_usuario
   DB_PASSWORD=sua_senha
   DB_DSN=seu_dsn


3. **Instale as dependências**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Execute o projeto**:
   ```bash
   python src/main.py
   ```

5. **Execute o projeto no Wokwi**:

Você pode visualizar e interagir com a simulação do projeto no Wokwi clicando no link abaixo:

[![Simulação no Wokwi](wokwi\circuito_diagrama.png)](https://wokwi.com/projects/413777804461865985)

Clique na imagem acima ou [aqui](https://wokwi.com/projects/413777804461865985) para acessar a simulação.

## 🗃 Histórico de lançamentos
* 0.3.0 - 16/10/2024
    * Adição do modelo de previsão de necessidades
* 0.2.0 - 14/10/2024
    * Adição do MER/DER e do DDL
* 0.1.0 - 12/10/2024
    * Criação do MER/DER e do README.md
* 0.0.1 - 10/10/2024
    * Criação do repositório e início do projeto

## Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>

