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

Em resumo, a análise dos dados mostra a complexidade e dinâmica do mercado de jogos eletrônicos, destacando a importância da adaptação às mudanças tecnológicas, a diversificação das opções para os jogadores e a influência de múltiplos fatores nas vendas de jogos. Esses dados fornecem uma ideia para entender as tendências e tomar decisões estratégicas no setor de jogos eletrônicos.

**Sobre Perfil de Usuários por região:**

Com base nas análises dos mercados de videogames na América do Norte, Europa e Japão, algumas conclusões claras emergem, evidenciando as dinâmicas regionais e as estratégias das empresas no setor.

Primeiramente, a liderança da Microsoft na América do Norte, com sua plataforma Xbox 360, demonstra sua forte presença nesse mercado, apesar da competição acirrada com outras fabricantes. Esse cenário indica um ambiente altamente competitivo, onde a Microsoft mantém uma fatia significativa das vendas.

No mercado europeu, observamos um equilíbrio entre as plataformas, com uma competição intensa entre as empresas. A Microsoft rivaliza de perto com as fabricantes japonesas, que continuam a dominar a região em termos de participação nas vendas.

Por outro lado, o mercado japonês é fortemente dominado pelas empresas de origem japonesa, com uma preferência local evidente por produtos domésticos. A presença mínima da Microsoft nesse mercado destaca essa preferência, demonstrando a importância da compreensão das especificidades culturais e do comportamento do consumidor em cada região.

Além disso, as análises revelam diferenças significativas nas preferências dos jogadores entre as regiões. Enquanto os gêneros de ação e esportes são populares na América do Norte e Europa, o Japão tem uma preferência mais forte por jogos de RPG. Essas divergências refletem uma variedade de fatores, incluindo cultura, tradições de jogos e preferências do público-alvo.

A prevalência da classificação "E" (para todos) em todas as regiões sugere uma preferência generalizada por jogos adequados para todas as idades. As classificações "T" (adolescentes) e "M" (mature) também são populares, embora sua importância varie dependendo da região. Por outro lado, as classificações menos comuns, como "EC" (early childhood) e "AO" (adults only), têm uma presença muito limitada nas vendas globais de jogos.

Em resumo, essas análises destacam a importância da compreensão das preferências regionais e da concorrência no setor de videogames. Elas demonstram como diferentes empresas conseguem competir e se posicionar de forma estratégica em mercados distintos, enfatizando a necessidade de adaptação às nuances culturais e preferências dos consumidores em cada região.

**Testando Hipóteses:**

Com base nos resultados dos testes de hipótese realizados para as plataformas 'xb' e 'pc', bem como para os gêneros 'action' e 'sports', podemos chegar a algumas conclusões importantes.

Primeiramente, para as plataformas 'xb' (Xbox) e 'pc' (computador pessoal), encontramos evidências estatísticas significativas que nos levam a rejeitar a hipótese nula. Isso sugere que as médias das classificações dos usuários para essas duas plataformas são diferentes. Essa diferença estatisticamente significativa pode indicar divergências na satisfação dos usuários ou na popularidade entre as plataformas, destacando a importância de considerar as preferências e experiências dos jogadores ao escolherem entre essas opções de jogo.

Por outro lado, para os gêneros 'action' e 'sports', não encontramos evidências suficientes para rejeitar a hipótese nula. Isso significa que não podemos concluir que há uma diferença estatisticamente significativa nas classificações médias dos usuários entre esses dois gêneros. Essa falta de diferença estatisticamente significativa sugere que, com base nos dados analisados, os usuários não têm uma preferência clara entre os gêneros 'action' e 'sports' em termos de classificações médias.

Em resumo, enquanto as diferenças nas classificações médias dos usuários entre as plataformas 'xb' e 'pc' são estatisticamente significativas, não podemos fazer a mesma afirmação para os gêneros 'action' e 'sports'. Essas conclusões destacam a importância de compreender as nuances das preferências dos usuários e fornecem insights valiosos sobre as dinâmicas do mercado de videogames, auxiliando na tomada de decisões estratégicas relacionadas a plataformas e gêneros de jogos.
