# Extrator de Avaliações Semanais do Google Maps
**Introdução**

Este projeto consiste em um script Python para automatizar a extração de avaliações de estabelecimentos no Google Maps. O objetivo principal é coletar as avaliações da semana anterior (de segunda-feira a domingo), processá-las e salvar os dados relevantes em um arquivo CSV para fácil análise e monitoramento.

**Recursos**

Extração Automatizada: Busca avaliações de um ou mais estabelecimentos de forma automática.

Filtragem por Período: O script calcula e filtra automaticamente as avaliações pertencentes à semana completa anterior.

Dados Estruturados: Salva as informações mais importantes (nome do estabelecimento, autor, nota, texto e data) em um arquivo CSV.

Nomenclatura Dinâmica: O arquivo de saída é nomeado dinamicamente com o intervalo de datas da extração, facilitando a organização.

**Tecnologias Utilizadas**

Python

Outscraper API → para a extração dos dados do Google Maps.

Pandas → para manipulação, filtragem e exportação dos dados.

Jupyter Notebook → para execução interativa do código.

**Como Usar**

Clone este repositório em sua máquina local:


git clone https://github.com/seu-usuario/seu-repositorio.git
Instale as dependências necessárias. Crie um arquivo requirements.txt com o conteúdo abaixo:

pandas
outscraper
E execute o comando de instalação:


pip install -r requirements.txt
Configure o script:

Abra o notebook API_OUTSCRAPER_AVALIAÇÕES.ipynb.

Insira sua chave da API da Outscraper na variável API_KEY.

Adicione as URLs dos estabelecimentos que você deseja monitorar na lista locais_para_pesquisar.

Execute o notebook:

Rode todas as células do notebook para iniciar a extração. Ao final, um arquivo CSV com o nome avaliacoes_AAAA-MM-DD_a_AAAA-MM-DD.csv será gerado no mesmo diretório.

Estrutura do Arquivo de Saída
O arquivo CSV gerado conterá as seguintes colunas:

name: Nome do estabelecimento avaliado.

author_title: Nome do autor que fez a avaliação.

review_rating: A nota da avaliação (de 1 a 5).

review_text: O conteúdo textual da avaliação.

review_datetime_utc: A data e hora em que a avaliação foi publicada (em formato UTC).

**Contribuições**

Contribuições para este projeto são bem-vindas. Se você tiver sugestões, melhorias ou encontrar algum problema, sinta-se à vontade para abrir uma issue ou enviar um pull request.

**Contato**

Para dúvidas ou perguntas relacionadas a este projeto, entre em contato com Gabriel Veloso via e-mail: 📩 velosogabriel5@gmail.com
