# MovieLens 1M
O GroupLens Research (http://grouplens.org/datasets/movielens) fornce várias coleções de dados de avaliações de filmes 
obtidos de usuários do MovieLens no fim dos anos 1990 e início dos anos 2000. Os dados contêm avaliações de filmes, 
metadados (gêneros e ano) e informações demográficas sobre os usuários (idade, código postal, identificação de gênero 
e profissão).

O conjunto de dados MovieLens 1M contém um milhão de avaliações coletadas de 6 mil usuários sobre 4 mil filmes.

## Descrições dos arquivos
### Ratings
Todas as avaliações estão contidas no arquivo "ratings.dat" e estão no seguinte formato:

`UserID::MovieID::Rating::Timestamp`

- UserIDs variam entre 1 e 6040 
- MovieIDs variam entre 1 e 3952
- Ratings são feitas em uma escala de 5 estrelas (somente avaliações com estrelas inteiras)
- Timestamp é representado em segundos desde a época, conforme retornado por time(2)
- Cada usuário tem pelo menos 20 avaliações

### Users
As informações do usuário estão no arquivo "users.dat" e estão no seguinte formato:

`UserID::Gender::Age::Occupation::Zip-code`

Todas as informações demográficas são fornecidas voluntariamente pelos usuários e são não verificado quanto à precisão. 
Somente usuários que forneceram alguns dados demográficos informações estão incluídas neste conjunto de dados.

- Gender é indicado por um “M” para masculino e “F” para feminino
- Age é escolhida entre as seguintes faixas:
    * 1: "Menores de 18 anos"
	* 18: "18-24"
	* 25: "25-34"
	* 35: "35-44"
	* 45: "45-49"
	* 50: "50-55"
	* 56: "56+"
- Occupation é escolhida entre as seguintes opções:
	* 0: “outro” ou não especificado
	* 1: “acadêmico/educador”
	* 2: "artista"
	* 3: "clerical/administrador"
	* 4: "estudante universitário/de pós-graduação"
	* 5: "atendimento ao cliente"
	* 6: "médico/assistência médica"
	* 7: "executivo/gerencial"
	* 8: "agricultor"
	* 9: “dona de casa”
	* 10: "Aluno do ensino fundamental e médio"
	* 11: "advogado"
	* 12: "programador"
	* 13: "aposentado"
	* 14: "vendas/marketing"
	* 15: "cientista"
	* 16: “autônomo”
	* 17: “técnico/engenheiro”
	* 18: “comerciante/artesão”
	* 19: "desempregado"
	* 20: "escritor"

### Movies
As informações do filme estão no arquivo "movies.dat" e estão no seguinte formato:

`MovieID::Title::Genres`

- Title são idênticos aos títulos fornecidos pelo IMDB (incluindo
ano de lançamento)
- Genres são separados por tubos e selecionados entre os seguintes gêneros:
    * Action
	* Adventure
	* Animation
	* Children's
	* Comedy
	* Crime
	* Documentary
	* Drama
	* Fantasy
	* Film-Noir
	* Horror
	* Musical
	* Mystery
	* Romance
	* Sci-Fi
	* Thriller
	* War
	* Western
- Alguns MovieIDs não correspondem a um filme devido a duplicação acidental entradas e/ou entradas de teste
- A maioria dos filmes é inserida manualmente, portanto podem existir erros e inconsistências
