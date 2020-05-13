# Projeto-Dey
Projeto Dey
Estou estudando ciência de dados nessa quarentena e achei uma ótima ideia tentar aplicar meus conhecimentos em exemplos reais  usando uma grande base de dados juntamente com o python.

Meu irmão trabalha numa empresa de abastecimento de água e a empresa estava com a seguinte dúvida qual que deve ser o dimensionamento do hidrômetro e da tubulação para a construção de X áreas residenciais na região (Se o hidrômetro e a tubulação não forem dimensionados corretamente pode acontecer de a água não ser distribuída corretamente).

Com isso a empresa forneceu uma tabela de clientes, onde fornece vários tipos de informações sobre eles e dessas informações são 5 que nos interessam:
Número de áreas residenciais
Número de áreas comerciais 
Número de áreas indústriais
Volume lido total 

▪ Então o primeiro passo que vamos fazer e abrir esse DataFrame e selecionar essas colunas
▪ Nesse data frame , não da pra saber quanto é o volume  de cada área só conseguimos saber de todas as áreas juntas(por exemplo uma pessoa pode ter registrado em seu nome 1 área residencial e 1 comercial o volume lido sera a soma dos dois volumes lidos)
▪ Então criei um novo data frame, onde é um data frame onde o as colunas de áreas indústriais e comerciais são iguais a 0. Fiz isso porque se temos como único valor a área residencial sabemos que o volume é específico dessa área
