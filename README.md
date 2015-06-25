# Espelho Político
=======
[![Code Climate](https://codeclimate.com/github/EspelhoPolitico/espelho-politico/badges/gpa.svg)](https://codeclimate.com/github/EspelhoPolitico/espelho-politico)
=======

É um website desenvolvido em Ruby on Rails durante as disciplinas de Métodos de Desenvolvimento de Software e Gestão de Portifólios e Projetos da Universidade de Brasília. Foi implementado com base no conceito de Dados Abertos, onde seu principal objetivo é mostrar, de forma transparente, para a população quais os políticos que realmente estão fazendo a diferença. Isso é demonstrado através de gráficos com a quantidade e nomes de proposições de leis criadas por eles e rankings dos que mais elaboram essas proposições. 

# Dependências

- Implantação do ambiente (https://github.com/EspelhoPolitico/automacao)

# Instalação

1. Entrar na máquina virtual: '$ vagrant ssh'
2. Clonar o repositório na pasta compartilhada: '$ cd /vagrant'
3. Entrar na pasta do projeto: '$ cd espelho-politico'
4. Rodar o comando '$ bundle install'
5. Entrar na pasta de configuração: '$ cd /config'
6. Mudar o arquivo: '$ mv database.yml.template database.yml'
7. Entrar no arquivo de configuração: '$ vi database.yml'
8. Adicionar, após a linha timeout: 'username: root', e abaixo dessa: 'password: root123'
9. Sair da pasta de configuração: '$ cd ..'
9. Rodar o comando 'rake db:create'
10. Rodar o comando 'rake db:migrate'
11. Rodar a aplicação através do comando 'rails s'

# Parser

Para rodar o parser basta:

1. Entrar na pasta do parser: 'cd parser'
2. Rodar o comando: 'python parser.py ep_dev root root123'

**Observação:** O parser demora muito para finalizar completamente.
