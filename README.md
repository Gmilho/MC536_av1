# MC536: Primeira Avaliação
Primeiro projeto para a matéria MC536, oferecida no 1º semestre de 2025 pelo [Instituto de Computação da Universidade Estadual de Campinas (UNICAMP)](https://ic.unicamp.br/), e ministrada pelo docente [Breno Bernard Nicolau de França](https://ic.unicamp.br/docente/breno-bernard-nicolau-de-franca/).  
  
Este projeto é autoria de:
  - [Daniel Baltieri Ismael (247855)](https://github.com/DBisma)
  - [Gustavo Costa Salles Silva (198487)](https://github.com/gu-css)
  - [João Emílio Ferreira (247184)](https://github.com/Gmilho/)

## Objetivos e Decisões

## Resultados
[Colocar imagens]

## Obtendo Dependências e Executando
Este projeto depende de [Python 3](https://www.python.org/), [Pip](https://pypi.org/project/pip/), [Jupyter](https://jupyter.org/), [Psycopg 2](https://www.psycopg.org/docs/) e [Postgre-SQL](https://www.postgresql.org/).
No sistema operacional Ubuntu e em seus similares, as instruções para obtenção dessas dependências são:

1. Abra seu emulador de terminal de preferência e certifique-se de possuir _Python 3_ e _pip_ instalados com os comandos `python3 --version` e `pip --version`; baixe os dois caso não possua.
2. Postgre-SQL também é necessário, e pode ser obtido com o comando `sudo apt install postgresql` em distribuições baseadas em Ubuntu.
3. Escolha um diretório para armazenar o ambiente e suas as dependências com o comando: `python3 -m venv <caminho>` (e.g. `python3 -m venv /home/username/Documents/python3-Envs/proj1`);
4. Selecione o ambiente criado com o comando `source <caminho>/bin/activate` (e.g. `source /home/username/Documents/python3-Envs/proj1/bin/activate`);
5. Uma vez selecionado, utilize os comandos `pip install psycopg2` ou `pip install psycopg2-binary` e `pip install jupyter` para instalar as demais dependências.
6. Inicialize o processo de Postgre-SQL. Em um sistema baseado em Ubuntu utilizando _systemd_, isso pode ser feito pelo comando `sudo systemctl start postgresql`.
7. O status pode ser verificado com `sudo systemctl status postgresql`, também em sistemas que utilizam _systemd_.
8. Agora, usaremos o programa para criar nossos bancos de dados. Ainda pelo terminal, o comando `sudo -u postgres psql` entra no usuário padrão.
9. Depois disso, execute os comandos  
`CREATE DATABASE ava1_db;`  
`CREATE USER ava1_user WITH PASSWORD 'ava1_password';`  
`GRANT ALL PRIVILEGES ON DATABASE ava1_db TO ava1_user;`  
e saia com `\q`.
10. Navegue até o diretório em que clonou este projeto (e.g: `cd /home/username/Documents/GitHub/MC536_Av1`)
11. Execute o comando `jupyter notebook`, que deverá abrir um explorador de arquivos em seu navegador.
12. Selecione o projeto **_ava_um_notebook.ipynb_**;
13. Por fim, basta executar os blocos de código do sequencialmente. Comece pelo começo, vá até o final, e então pare. Os resultados são exibidos na própria página.

## Créditos e Agradecimentos
_Datasets_ ([1](https://repositorio.seade.gov.br/dataset/infraestrutura-e-meio-ambiente/resource/f175c301-b9c9-46d0-9522-1e1f7134846c?inner_span=True),[2](https://repositorio.seade.gov.br/dataset/infraestrutura-e-meio-ambiente/resource/abf3787f-5d6c-4f63-81e0-79021464b6c4)) disponibilizados publicamente pelo SEADE.  
Agradecimentos especiais aos nossos PADs pela paciência infinita demonstrada durante o semestre para com este grupo.
