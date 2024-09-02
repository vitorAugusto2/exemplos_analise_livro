# Nomes de bebês americanos de 1880 a 2010
A SSA (Social Security Administration, Administração de Securtidade Social) dos Estados Unidos disponibiliza dados sobre 
frequência de nomes de bebês desde 1880.


## Descrição do arquivo
Para cada ano de nascimento AAAA após 1879, criamos um arquivo delimitado por vírgulas chamado yobAAAA.txt, na pasta "babynames". 
Cada  registro nos arquivos anuais individuais tem o formato `name, sex, number`, onde:

- **name:** nome entre 2 a 15 caracteres
- **sex:** M (masculino) ou F (feminino)
- **number:** número de ocorrências do nome
  
Cada arquivo é classificado primeiro por sexo e depois por número de ocorrências em ordem decrescente. Quando há empate no número de ocorrências, os nomes são listados em ordem alfabética ordem. Essa classificação facilita a determinação da classificação de um 
nome. O primeiro registro para cada sexo foi classificação 1, o segundo registro para cada sexo tem classificação 2 e 
assim por diante. Para salvaguardar a privacidade, restringimos a nossa lista de nomes àqueles com pelo menos 5 ocorrências.