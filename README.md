# KM WebApp

## Como desenvolver?

1. Clone o repositório;
2. Crie um pipenv com Python 3.8.1;
3. Ative o pipenv;
4. Instale as dependências;
5. Configure a instância com o .env;
6. Rode a aplicação.

```console
# 1
git clone git@github.com:marcospatzer/meuPrimeiroProjeto.git
cd meuPrimeiroProjeto

# 2
__Antes de rodar o comando, verificar se o python e o pipenv esta instalado na máquina.__
# Lembre-se de verificar se o python global é o correto antes de rodar o comando abaixo!
pipenv --three  # Este comando gera uma .venv no repositório!

# 3
pipenv shell

# 4
pipenv install

# 5
# Após rodar o comando abaixo abra o arquivo ".env" em seu editor favorito e configure os parâmetros antes de continuar!
cp contrib/env-sample .env

# 6
python manage.py runserver
```

---
## Instalações
Como instalar o pipenv.

*No Windows*
Abra o PowerShell como administrador e rode o seguinte comando:
```python
pip install --upgrade pip

set PATH=%PATH%;set PATH=%PATH%;'c:\users\SEU_USUARIO\appdata\local\programs\python\python38-32\Scripts'
```

---
## Comandos úteis

APAGAR os dados do banco exeto a tabela de migrações.  
_Útil para atualizar banco de testes_

```python  
python manage.py flush
```

---
## A fazer
- Criar forma de mostrar projeto padrão podendo mudar de forma que toda vez que fizer login volte o padrão
- Projeto e Portadores trazer os que o usuário tem acesso
- Na grid filtrar por projetos liberados para o usuário
- Colocar help_text nos campos do modelo "tesouraria.Fbordero"
- Campo "pro" do modelo "Fbordero" só pode trazer os projetos que o usuário tem disponível e vir padrão o atual do menu.
- Aumentar tamanho do .aligned label
- Tentar reduzir o espaçamento entre linhas

- Pegar com Giba 4 novos campos para o modelo "cadastros.Dbanco"
- Reordenar os campos da tela (GIBA VAI FAZER)