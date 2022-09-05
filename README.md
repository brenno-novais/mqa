# Montagem do Setup

1. Instalar o [Python (3.10.0)](https://www.python.org/downloads/release/python-3100/)
2. Clonar este repositório
3. Criar um virtual environment
   Digite, no prompt de comando, na pasta onde você clonou o repositório: <code>pipenv install</code>
4. Após isso, ative o venv, digitando: <code>pipenv shell</code>
   Necessário toda vez que for usar o setup
5. Instale o Jupyter Notebook (<code>pip install jupyter-lab</code>)
6. Instale os seguintes pacotes (basta dar um pip install seguido do nome deles em letra minúscula):
   - Numpy
   - Pandas
   - Matplotlib
   - Seaborn
   - Sklearn
7. Digite no prompt <code>jupyter-lab</code> para iniciar

# Sobre o dataset

O dataset contém dados sobre músicas e usuários do Spotify até o ano de 2018. Pode ser acessado pelo seguinte [link](https://www.aicrowd.com/challenges/spotify-sequential-skip-prediction-challenge). Foi feito um recorte dos dados, para que trabalhassemos com um número de 1015 linhas de informação.

A descrição de cada variável está no arquivo descricao_das_variaveis.pdf. Abaixo, as variáveis que utilizaremos no nosso dataset.

    Variavéis quantitativas
    - [duration] Duração (em segundos)
    - [us_popularity_estimate] Estimativa de popularidade nos EUA
    - [danceability] Dançabilidade
    - [energy] Energia
    - [instrumentalness] Instrumentalidade

    Variáveis qualitativas:
    - [release_year] Ano de Lançamento
    - [mode] Escala musical
    - [skip_1] Música foi pulada no início
    - [not_skipped] Música não foi pulada
    - [hour_of_day] Escutada em qual hora do dia

    Variável de identificação
    - [track_id | track_id_clean] ID da música

# Algumas perguntas motivadoras:

    - Detalhes da música como duração, dançabilidade, energia, instumentalidade influenciam no "pulo" da música por parte do usuário?
    - Existe um padrão para o tipos de música (alegre, dançante ...) que são escutados pelos usuários em uma determinada hora do dia?
    - O ano influencia no "pulo" da música?
    - Existe um padrão do tipo de música e do ano ao qual ela foi lançada?
    - Há preferências dos usuários por músicas em alguma esclaa específica?

# Bibliografia

Dataset:
@inproceedings{brost2019music, title={The Music Streaming Sessions Dataset}, author={Brost, Brian and Mehrotra, Rishabh and Jehan, Tristan}, booktitle={Proceedings of the 2019 Web Conference}, year={2019}, organization={ACM} }
