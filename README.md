# Games_Analysis
Você trabalha para a loja online Ice, que vende videogames no mundo todo. As avaliações de usuários e especialistas, gêneros, plataformas (por exemplo, Xbox ou PlayStation) e dados históricos sobre vendas de jogos estão disponíveis em fontes abertas. Você precisa identificar padrões que determinam se um jogo tem sucesso ou não. Isso vai permitir que você identifique possíveis sucessos e planeje campanhas publicitárias.

Os dados disponibilizados remontam a 2016. Vamos imaginar que estamos em dezembro de 2016 e você está planejando uma campanha para 2017.

(O importante é ter experiência trabalhando com dados. Realmente não importa se você está prevendo as vendas de 2017 com base nos dados de 2016 ou as vendas de 2027 com base nos dados de 2026.)

O conjunto de dados contém uma coluna de "rating" (classificação) que armazena a classificação ESRB de cada jogo. O Entertainment Software Rating Board avalia o conteúdo de um jogo e atribui uma classificação etária, como Teen (Adolescente) ou Mature (Adulto).

**Sobre os Dados:**

Durante a preparação dos dados, uma série de etapas foram realizadas para garantir que os dados estivessem limpos, organizados e prontos para análise.

Para começar, todos os nomes das colunas foram convertidos para minúsculas. Essa padronização na nomenclatura das colunas torna mais fácil e consistente o acesso aos dados.Além disso, todos os dados de texto foram convertidos para minúsculas. Isso foi feito para evitar duplicatas devido a diferenças de maiúsculas e minúsculas, garantindo uma análise mais precisa e completa dos dados.Após a conversão para minúsculas, foi realizada uma verificação para identificar e lidar com possíveis dados duplicados no dataframe. Isso foi feito para garantir a integridade dos dados e evitar redundâncias que poderiam distorcer os resultados da análise.

Em seguida, foram verificados os valores nulos em todas as colunas do dataframe. Os dados nulos da coluna 'Year_of_Release' foram tratados e convertidos para o tipo de dados inteiros, representando os anos de lançamento dos jogos. Da mesma forma, os dados nulos da coluna 'User_score' foram tratados e convertidos para o tipo de dados float, permitindo seu uso em cálculos numéricos.
Os dados nulos das colunas 'Critic_Score', 'Rating' e 'Name' foram tratados de acordo com a necessidade específica de cada coluna, utilizando técnicas adequadas para garantir a integridade dos dados.

Por fim, o rating ESRB (Entertainment Software Rating Board) foi padronizado para garantir consistência nos dados, simplificando a análise e a comparação entre os jogos com diferentes classificações.

Essas ações visam garantir que os dados estejam organizados e livres de inconsistências, possibilitando uma análise mais precisa.


**Analisando os Dados:**

A análise dos dados revela uma evolução dinâmica no cenário das plataformas de jogos eletrônicos ao longo das décadas, com mudanças significativas ocorrendo a partir da década de 1990. Plataformas que dominaram o mercado na década de 1980 foram substituídas por tecnologias mais avançadas, refletindo um ciclo de vida típico para essas plataformas.

Observamos um aumento na competição e diversidade de opções para os jogadores, com o surgimento de várias plataformas novas após a década de 1990. Esse crescimento contribuiu para um mercado mais equilibrado, onde várias plataformas disputam a atenção e os gastos dos consumidores.

Os histogramas evidenciam padrões recorrentes sugerindo um ciclo médio de vida para as plataformas de jogos eletrônicos, geralmente em torno de 10 anos, com exceção notável para os lançamentos para 'PC', que mostram um padrão de crescimento mais linear e prolongado ao longo de aproximadamente 20 anos.

A análise também destaca a dominação das três grandes fabricantes de consoles de videogame: Sony, Nintendo e Microsoft. Essas empresas lançaram sucessivas plataformas ao longo dos anos, demonstrando sua capacidade de adaptação às mudanças e avanços tecnológicos no setor.

Em relação às vendas de jogos, observamos uma ampla dispersão nos dados, indicando uma variedade considerável nos valores das vendas. As correlações entre as avaliações dos profissionais e dos usuários com as vendas totais sugerem uma relação moderada a fraca, indicando que outros fatores além das avaliações influenciam as vendas de jogos.

Os gêneros de maior sucesso de vendas tendem a estar associados à classificação etária 'M' ('maduro'), enquanto os gêneros de menor sucesso não apresentam uma relação clara com faixas etárias específicas.
