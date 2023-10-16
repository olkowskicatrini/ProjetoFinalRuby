# Rails Cheat Sheet

## Vagrant

- **vagrant**: Comando para gerenciar ambientes de desenvolvimento virtual (VM).
- **up**: Inicia a máquina virtual definida no Vagrantfile.
- **suspend**: Pausa a máquina virtual.
- **halt**: Para a máquina virtual.
- **ssh**: Estabelece uma conexão SSH com a máquina virtual, permitindo interagir com ela, executar comandos e realizar configurações.

## Instalar gem

- **gem install rails -v 5.2.8**: Inicializa o sistema de gerenciamento de gemas (pacotes Ruby) para instalar a gema Ruby on Rails na versão 5.2.8.

## RVM (Ruby Version Manager)

- **rvm list**: Lista as versões do Ruby instaladas no sistema via RVM.
- **rvm list known**: Lista as versões do Ruby conhecidas disponíveis para instalação.
- **rvm install 2.3**: Instala uma versão específica do Ruby, por exemplo, a versão 2.3.
- **rvm use 2.6**: Define a versão especificada do Ruby (2.6) como ativa para comandos futuros.

## Criar um Projeto Rails

- **rails new nome_do_projeto -d postgresql**: Cria um novo projeto Ruby on Rails (substitua `nome_do_projeto` pelo nome desejado) com o banco de dados PostgreSQL como padrão.

## Iniciar o Servidor de Desenvolvimento

- **rails server -b 0.0.0.0 -e development**: Inicia o servidor de desenvolvimento do Rails, ou seja, o "rails server," e configura-o para ouvir em todas as interfaces de rede disponíveis. Pode ser acessado de outras máquinas na mesma rede.

## Geradores

- **rails generate controller pagina_inicial**: Gera um controlador chamado `pagina_inicial`.
- **rails destroy controller pagina_inicial**: Remove o controlador `pagina_inicial`.
- **rails generate scaffold NomeModelo campo1:tipo campo2:tipo ...**: Cria automaticamente um modelo, controlador, visões e migração para um recurso com campos especificados.

## Console do Banco de Dados

- **rails dbconsole**: Inicia um console de banco de dados diretamente do Rails para executar comandos SQL e interagir com o banco de dados.

## Tarefas do Banco de Dados

- **rails -T db**: Lista comandos relacionados ao banco de dados no ambiente Rails.
- **rails db:create**: Cria um novo banco de dados.
- **rails db:drop**: Exclui o banco de dados.
- **rails db:migrate**: Executa migrações pendentes no banco de dados.
- **rails db:rollback**: Reverte a migração mais recente.
- **rails db:seed**: Preenche o banco de dados com dados iniciais definidos em 'db/seeds.rb'.
- **rails db:setup**: Cria o banco de dados, carrega o esquema e executa as migrações, tudo em um comando.
