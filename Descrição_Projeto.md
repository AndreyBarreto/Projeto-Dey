# Projeto-Dey
Estou estudando ciência de dados nessa quarentena e achei uma ótima ideia tentar aplicar meus conhecimentos em exemplos reais  usando uma grande base de dados juntamente com o python.

Meu irmão trabalha numa empresa de abastecimento de água e a empresa estava com a seguinte dúvida qual que deve ser o dimensionamento do hidrômetro e da tubulação para a construção de X áreas residenciais na região (Se o hidrômetro e a tubulação não forem dimensionados corretamente pode acontecer de a água não ser distribuída corretamente, podendo ocorrer vazamentos também).

Com isso a empresa forneceu uma tabela de clientes, onde fornece vários tipos de informações sobre eles e dessas informações são 5 que nos interessam:

▪ Número de áreas residenciais
▪ Número de áreas comerciais 
▪ Número de áreas indústriais
▪ Número de áreas públicas
▪ Volume lido total 

▪ Então o primeiro passo que vamos fazer e abrir esse DataFrame e selecionar essas colunas, ja percebemos ao abrir que ela esta separada por ';' em vez de ',' , então informamos ao programa isso, também o arquivo está com problema de incoding, onde por meio de testes vi qual se adequava.

▪ Percebemos também que tem muitos valores NaN(valores não preenchidos) então substituo esses valores por 0, pois depois de consultar vi que os valores prenchidos com NaN são que não tem nada, ou seja 0

▪ Nesse data frame , não da pra saber quanto é o volume  de cada área só conseguimos saber de todas as áreas juntas(por exemplo uma 
pessoa pode ter registrado em seu nome 1 área residencial e 1 comercial o volume lido sera a soma dos dois volumes lidos)

▪ Então criei um novo data frame, onde é um data frame onde das colunas de áreas indústriais,comerciais e públicas são iguais a 0. Fiz isso porque se temos como único valor a área residencial sabemos que o volume é específico dessa área, mesmo excluindo essa quantidade de dados ainda continua uma boa quantidade de dados.

▪ Depois de ja ter o dataframe com o volume lido em relação ao número de áreas residenciais plotei um grafíco, onde o eixo das abcissas é o número de áreas residenciais e das ordenadas o Volume lido total, com isso obtemos uma correlação forte positiva(86%), ou seja esses dados tem uma forte relação entre eles.

▪ Plotei uma regressão linear no gráfico e descobri a equação da reta 

▪ Resposta= 12.13890353 + 7.94043072*(Número de áreas residenciais desejadas)

▪ Por exemplo uma construra vai fazer um condominio com 12 casas residenciais -> Resposta= 12.13890353 + 7.94043072*(12)

▪ 107.42407223 é o Volume lido total, ou seja o dimensionamento do hidrômetro e a tubulação serão em relação a esse volume se uma construra decidir fazer um condominio com 12 casas 


 



