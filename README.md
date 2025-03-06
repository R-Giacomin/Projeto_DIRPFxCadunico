# **Proposta de contrução de preditor de renda para os municípios a partir de registros administrativos**
# **Introdução**
As expectativas com a elaboração de indicadores, anualmente atualizáveis, de renda e de desigualdade a partir de dados regionalizados da quantidade de declarações de imposto de renda, por um lado, e de número de famílias e pessoas cadastradas no Cadastro Único para Programas Sociais do Governo Federal, por outro, giram em torno da possibilidade de aferir e identificar as porções territoriais regionais que apresentam uma maior densidade populacional em baixa renda, bem como as discrepâncias de renda a partir da separação das estatísticas de declarantes e de cadastrados.

Em que pese a complexidade da realidade e a possibilidade de distintas configurações na prática, a modelagem matemática da estatística de cotejamento entre os dados de declarantes e de cadastrados assenta-se, em última instância, no pressuposto de que a quantidade de pessoas (titulares e dependentes) que emitem as declaração de imposto de renda compõem as famílias com condições de rendimentos suficientes e que ultrapassam os limites de isenção, sendo, portanto, as de maior renda; por outro lado, as famílias (e pessoas) cadastradas no CadÚnico compõem a parcela populacional mais vulnerável do ponto de vista da renda, configurando-se, via de regra, o contingente que mais necessita das políticas e programas estatais de transferência de renda para aferir melhores condições de vida.

O exercício consiste em analizar dois indicadores municipais calculados a partir de dados administrativos, o percentual de pessoas com renda até meio salário mínimo cadastradas no Cadúnico, o percentual de pessoas em famílias declarantes do IRPF e os rendimentos totais das DIRPFs per capita. Tais indicadores fazem analogia a "taxa de pobreza" e "taxa de riqueza" dos municípios. Através da combinação desses indicadores espera-se estimar o rendimento domiciliar per capita dos municípios para fins de planejamento, monitoramento e avaliação de políticas de desenvolvimento regional.
## **Objetivo**
Proposição de indicadores de renda e desigualdade em nível municipal, com disponibilidade anual (frequência maior do que o Censo Demográfico – IBGE), utilizando-se, preferencialmente, de registros administrativos oficiais.
## **Justificativa**
O território é extremamente dinâmico em suas mais diversas facetas, de modo que iniciativas e ações individuais ou coletivas de cunho socioeconômico, de gênese espontânea ou estruturadas em planejamentos públicos ou privados robustos, podem ensejar modificações mais ou menos amplas nas oportunidades e realidades de desenvolvimento de uma dada região.

Nesse sentido, os retratos decenais censitários não permitem um monitoramento tempestivo dos dinamismos inerentes às modificações territoriais, sobretudo na dimensão econômica em escala regionalizada (centrada, sobremaneira, na análise da renda), sendo, pois, limitados por sua periodicidade de disponibilidade no que tange à eficácia de indicadores voltados à avaliação das políticas públicas de desenvolvimento regional.

Diante disso, faz-se necessário pensar em dados cujas disponibilidades são mais adequadas do que os Censos Demográficos para a avaliação da condição de renda e de desigualdade dos municípios, sob o fulcro de acompanhar, de modo mais sinérgico e ativo, as condições e respectivas modificações, ao longo do tempo, do dinamismo e/ou estagnação econômica de um dado recorte municipal em escala regional. Assim, favorece-se, em última instância, uma elegibilidade mais assertiva dos espaços-alvo das políticas públicas fomentadas pela Política Nacional de Desenvolvimento Regional - PNDR.

A partir disso, torna-se possível pensar, ancorado em dados oficiais institucionais no âmbito da Administração Pública Federal, em bases de dados alternativas para diagnosticar a situação de renda – e, a partir dela, as relações intra e inter-regionais de desigualdade – de um dado município no cenário nacional.

Duas bases potenciais, a serem sumariamente descritas a seguir, referem-se: (i) à Declaração do Imposto sobre a Renda da Pessoa Física (DIRPF), sob tutela da Secretaria Especial da Receita Federal do Brasil do Ministério da Fazenda; e (ii) ao Cadastro Único para Programas Sociais (CadÚnico), do Ministério do Desenvolvimento e Assistência Social, Família e Combate à Fome.
## **Metodologia**
Inicialmente é realizado o trabalho de indentificação, leitura, limpeza, organização e consolidação os dados de diversas tabelas para calculo dos indicadores necessários para a análise.

Para esse fim foram utilizadas as seguintes tabelas:
- Censo demográfico 2010 - tabela de rendimento domiciliar per capita por município;
- Censo demográfico 2010 - tabela de população residente por município;
- Censo demográfico 2010 - tabela de total de domicílios permanentes por município;
- Base de dados - tabela com diversas classificações municipais;
- Cadastro Único 2010 - tabela do total de famílias cadastradas por município (idealmente, seria utilizar total de pessoas em famílias com renda per capita até meio salário-minimo atualizadas, porém esses dados não estão disponíveis de forma aberta para 2010);
- Grandes números da DIRPF 2010 - tabela de agregados municipais.
- Tabela de:para para identificação dos códigos dos municípios da tabela da DIRPF.

Após a consolidação das tabelas e exclusão dos dados faltantes, foram calculados os indicadores:
- Participação do Cadúnico nos municípios: Total de famílias cadastradas (Cadúnico) / Total de domicílios (Censo), nomeado como **"Taxa de Cadúnico"**;
- Participação do IRPF nos municípios - Estimativa do número de pessoas em famílias declarantes do IRPF (Grandes números da DIRPF) / população residente (Censo), nomeado como **"Taxa de IRPF"**;
- Total de rendimentos declarados na DIRPF (Grandes números da DIRPF) / população residente (Censo), nomeado como **"Rpc IRPF"**.

Também foi criada variável de **quintil do rendimento domiciliar per capita** dos municípios (Censo) para fins de análise descritiva dos dados.
