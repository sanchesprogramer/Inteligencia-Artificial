# Utilização de Machine Learning para fornecer dados estratégicos para prevenção e mitigação de desastres naturais com o uso de gráficos para tomada de decisão.

 
Felipe de Almeida Parreira
Raphael Dias Sanches
Gabriel William Pauleti
Davi de Carvalho Sampaio

1Faculdade de Computação e Informática (FCI) Universidade Presbiteriana Mackenzie – São Paulo, SP – Brasil
2Programa de pós-graduação em Computação Aplicada – Faculdade de Computação e Informática (FCI) – Universidade Presbiteriana Mackenzie – São Paulo, SP – Brasil
 
{10400771, 10403418, 10400878, 42337004}@mackenzista.com.br
 
 
Palavras-chave: Machine learning, IA , IOT, desastres naturais, mitigação de desastres
 
 
# 3.   	Resumo

Esse projeto utilizará os dados de datasets de para o aprendizado de máquina (Machine Learning, ML)(DUC, 2020)  para a construção de uma Inteligência Artificial (Artificial Inteligence, IA) que terá como objetivo prever quando poderá haver uma inundação com foco no desastre que ocorreu no Rio Grande do Sul. Para isso, utilizaremos métodos como um centro de mitigação que terão especialistas analisando os dados recebidos da IA, esses dados serão convertidos em gráficos utilizando a lógica Fuzzy(ADALZAHER, 2022) o que facilitará a decisão se será necessário ou não alertar a população de uma possível inundação.Os alertas serão feitos através de alarmes inteligentes (Smart alarms)(ASIF, 2023) que informarão a população da região sobre a possível inundação da região, permitindo assim, que vidas e diversos itens sejam salvos desse desastre.

# 4.   	Introdução

O projeto surge para enfrentar os desafios impostos pela natureza como resposta aos desafios impostos por desastres naturais, especialmente inundações como por exemplo a inundação do Rio Grande do Sul onde 876 mil pessoas foram afetadas negativamente perdendo suas casas, animais de estimação e, muitas vezes, até suas vidas por causa da inundação ocorrida no dia 27 de abril de 2024 (IPEA, 2024).
Diante desse cenário alarmante, a proposta do projeto é utilizar dados fornecidos por bases públicas, originados por dispositivos da Internet das Coisas (Internet Of Things, IOT) juntamente com técnicas de aprendizado de máquina (Machine Learning, ML) para que seja possível construir uma solução de monitoramento, previsão e até mesmo divulgação de alertas em tempo real. Essa abordagem geralmente gera e transmite dados precisos e relevantes para auxiliar a tomada de decisão de equipes e entidades competentes. A solução irá utilizar dados obtidos por IOT para que seja possível a captação de informações ambientais como nível de chuva e velocidade do vento. Geralmente ao ser detectado qualquer sinal de precipitação (ADALZAHER, 2022), um alerta é enviado para o algoritmo de aprendizado de máquina (Machine Learning, ML), que pode servir de base para uma Inteligência Artificial (IA) treinada. Essa IA será responsável por identificar padrões que antecedem eventos climáticos extremos. Com base nos dados analisados, o sistema irá gerar previsões de inundações, outros desastres associados e as áreas que serão mais afetadas. Como consequência, irá oferecer projeções sobre a possibilidade e a gravidade desses eventos em locais específicos. Para garantir a confiabilidade e a integridade dessas informações, os dados obtidos geralmente passam por uma avaliação de pontuação de confiabilidade de IOT (IoT Trustability Score, ITS), que irá verificar o nível de confiabilidade dos dados fornecidos pelo IOT, fornecendo assim um novo nível de segurança (SADANANDAN, 2021). Essa avaliação geralmente verifica a consistência e a precisão dos dados fornecidos pelos sensores. Com isso, será possível aumentar a confiabilidade dos alertas emitidos.
 
Segundo o artigo (KAVAK,2022) os dados podem ser convertidos em dados não binários utilizando a Lógica Fuzzy, que permitirá o processamento de informações incertas e pode auxiliar na interpretação dos resultados. Em seguida, os dados podem ser transmitidos para especialistas em um centro de mitigação de risco (ALHAMIDI, 2024) que validam as informações processadas e aprovam, ou não, a divulgação dos alertas. A comunicação dos resultados irá ocorrer por meio das redes sociais, outras plataformas digitais e até mesmo alarmes inteligentes (Smart alarms), com o objetivo de alcançar rapidamente o maior número de pessoas e permitir assim que a população e o governo tomem as medidas necessárias para segurança pessoal e coletiva (ASIF, 2023). O processo proposto busca aprimorar a resposta a desastres naturais e reduzir os impactos, proporcionando assim uma ferramenta poderosa de apoio à decisão para gestores e autoridades competentes envolvidas no gerenciamento de crises ambientais.
 
# 5.   	Descrição do Problema

O problema enfrentado é a falta de resposta eficiente em um tempo hábil e isso causava uma inevidência no combate aos desastres naturais, especialmente nas inundações. Esse acontecimento pode ser observado com mais clareza nas inundações do Rio Grande do Sul do dia 27 de abril de 2024. Os efeitos dessas catástrofes foram devastadoras pois tiveram muitas perdas de vidas humanas e não humanas, perda de moradias, perda de muitos investimentos que tinha na cidade e etc. Dito isso, o projeto tem como foco a incapacidade de prever com velocidade e precisão esses eventos, o que acarreta em uma perdas inestimáveis. hoje em dia a previsão de desastres naturais depende métodos mais arcaicos que não são tão eficazes por se tratar de um complexo entendimento dos dados da natureza. a falta de um sistema integrado com as redes sociais e um sistema que gera dados em gráficos de fácil leitura para especialistas acarreta em uma gestão de desastres naturais ineficiente e demorada. Portanto o projeto enfrenta um desafio em criar uma solução tecnológica que integre o monitoramento em tempo real, previsão de eventos externos e uma comunicação rápida e eficiente de alertas para toda população. 

# 6. Aspectos Éticos


Um dos aspectos importantes é o armazenamento de dados sensíveis, como o endereço do usuário por ser uma parte crucial do sistema. Os dados serão criptografados e armazenados em um banco de dados separados, e o acesso aos dados será restrito dentro do sistema para garantir a confidencialidade dos usuários. Para o tratamento de dados, os dados só serão utilizados para decidir qual será a área da comunicação de acordo com os dados meteorológicos presentes no sistema.
A IA será utilizada na questão de análise de dados, onde as chuvas serão analisadas ao longo do tempo para poder gerar a previsão do próximo 

# 7. Dataset

Nosso dataset foi retirado do site do governo (https://portal.inmet.gov.br/dadoshistoricos) referente ao estado do Rio Grande do Sul, mais especificamente da cidade de Porto Alegre - Jardim Botânico no período de 01/01/2024 a 31/12/2024 em que contém as seguintes colunas:
- Data (DD/MM/YYYY)
- Hora UTC (HHMM UTC)
- PRECIPITAÇÃO TOTAL, HORÁRIO (mm)
- PRESSÃO ATMOSFERICA MAX.NA HORA ANT. (AUT) (mB)
- PRESSÃO ATMOSFERICA MIN. NA HORA ANT. (AUT) (mB)
- RADIACAO GLOBAL (Kj/m²)
- TEMPERATURA DO AR - BULBO SECO, HORARIA (°C)
- TEMPERATURA DO PONTO DE ORVALHO (°C)
- TEMPERATURA MÁXIMA NA HORA ANT. (AUT) (°C)
- TEMPERATURA MÍNIMA NA HORA ANT. (AUT) (°C)
- TEMPERATURA ORVALHO MAX. NA HORA ANT. (AUT) (°C)
- TEMPERATURA ORVALHO MIN. NA HORA ANT. (AUT) (°C)
- UMIDADE REL. MAX. NA HORA ANT. (AUT) (%)
- UMIDADE REL. MIN. NA HORA ANT. (AUT) (%)
- UMIDADE RELATIVA DO AR, HORARIA (%)
- VENTO, DIREÇÃO HORARIA (gr) (° (gr))
- VENTO, RAJADA MAXIMA (m/s)
- VENTO, VELOCIDADE HORARIA (m/s)

# 8.   	Metodologia
 
O desenvolvimento de um sistema estruturado para cada fase de um desastre pode ser alcançado através de uma técnica de projeto em três etapas: pré-desastre, evento-desastre e pós-desastre (AMAJUOYI, 2020). No estágio pré-desastre, a predição é realizada por algoritmos de ML, IA e ITS, enquanto um segundo passo envolve o alerta, enviado por um Smart Alarm específico (AMAJUOYI, 2023). Durante o evento-desastre, autoridades são informadas, e comunicados são divulgados nas redes sociais para ampliar o alcance das informações (GHANSHALA, 2024). Finalmente, na fase pós-desastre, ocorre a reabilitação da área afetada, visando restabelecer a vida cotidiana dos moradores da região impactada.

Figura 1 – Comparação das fases interconectadas do ciclo de vida entre a gestão de desastres e a gestão de projetos Fonte: Amajuoyi, 2022, p. 03.
Inicialmente, é fundamental considerar aspectos geológicos e ambientais específicos de cada região (Delavar, 2023), como altitude, declividade, aspecto, curvaturas, distância até rios e estradas, tipo de solo, uso do solo, profundidade do solo, além de índices de precipitação e índices hidrológicos. A correta identificação dessas variáveis é essencial para entender a dinâmica de processos naturais, como a suscetibilidade a enchentes, especialmente diante do agravamento desse fenômeno em função das mudanças climáticas e das ações antrópicas, como o desmatamento, a urbanização desordenada e a ocupação de leitos de rios. Para a seleção das variáveis mais relevantes, normalmente são aplicadas técnicas de otimização e seleção de atributos, como o Feature Optimization Process (FOP), que é um processo genérico de otimização de variáveis (Delavar, 2023) e ou algoritmo Boruta, um método específico de seleção de atributos baseado em Random Forest (RF), visando aprimorar a escolha dos fatores que mais influenciam a ocorrência de enchentes.
O estudo propõe o uso de modelos híbridos e métodos de Ensemble (ADI, 2023) — combinação de vários algoritmos de ML — para melhorar a previsão da suscetibilidade a enchentes. Em especial, segundo o artigo (ADI,2023) geralmente são testados os métodos PRF (Parallel Random Forest), RRF (Regularized Random Forest) e ERT (Extremely Randomized Trees), que serão comparados com modelos tradicionais, como RF e BRT (Boosted Regression Trees), buscando reduzir problemas como overfitting e identificar de forma mais precisa as variáveis determinantes para a ocorrência de enchentes (BAND, 2020).
Dentro desse contexto de gerenciamento de desastres, é essencial destacar as inundações, que representam um dos desastres naturais mais recorrentes e devastadores. Os impactos das inundações são diversos, incluindo a destruição de casas, cidades inteiras, perdas humanitárias e materiais, como fazendas (G1,2024) . Além disso, inundações afetam profundamente o meio ambiente ao redor, transformando áreas inteiras. Pessoas e empresas fora da zona de risco podem contribuir com recursos para ajudar a região afetada, como roupas, comida e água. Redes sociais (GHANSHALA, 2024) desempenham um papel crucial nesse processo, facilitando a disseminação de informações e mobilizando ajuda para os moradores e esclarecendo os motivos do alerta.
Para fazer uma verificação as áreas inundadas é possível utilizar a tecnologia de radar SAR (AMITRANO, 2024), em que, por meio do radar, é emitido um sinal que, ao atingir uma área alagada, reflete de volta, indicando que a região está inundada, podendo ser um grande aliado ao governo para identificar áreas inundadas e fazer o resgate de seres humanos e animais.
Para que esse sistema de gerenciamento de desastres opere de forma eficiente, é necessário um modelo que permita a coordenação inteligente entre diferentes entidades, sensores, plataformas, pessoas, sistemas e algoritmos. Nesse contexto, o conceito de Process-of-Things (PoT) se torna relevante, pois oferece uma estrutura para organizar a colaboração entre seres vivos e não vivos, facilitando a descoberta, conexão, adaptação e avaliação contínua de seus comportamentos e capacidades. A aplicação do PoT (ALASKAR, 2020) permitiria, por exemplo, que sensores ambientais, algoritmos de predição e canais de comunicação se integrassem de maneira autônoma e dinâmica conforme a situação se desenvolvesse.
O tratamento dos dados virá a partir de 5 ajustes (ADI, 2023), que serão: limpeza de dados inválidos, redução dos dados (retirando os dados que não serão utilizados), scaling data, transformação de dados e particionamento de dados. Após o tratamento desses dados podem ter utilizado a lógica FUZZY para compreensão das variáveis para que assim seja possível a criação de árvores de decisão e gráficos de fácil entendimento levando em consideração essas variáveis.

Figura 2: Fluxograma simulado do projeto
Segundo o artigo (ABRAHAM, 2024) poderá ser feita a utilização da biblioteca SHAP do Python que auxilia a levar em consideração todos os resultados dos modelos de aprendizado de máquina. Portanto isso irá permitir testar todos os modelos (Regressão linear, Árvores de decisão, Florestas aleatórias, Modelos de aumento de gradiente e Redes neurais) para que assim seja possível verificar qual modelo se adapta melhor ao projeto. Geralmente o modelo de ensemble (RF, XGBoost e Stacking) traz um melhor desempenho se comparados com modelos individuais como SVM, KNN e Lasso (ABDELWAHAB, 2024), porém demoram muito tempo para ser treinados por levar em consideração inúmeras variáveis.


# 9. Resultados esperados

1. Irá permitir um monitoramento de uma cidade, estado ou até mesmo país em tempo real, pois com a implementação do sistema será possível um monitoramento contínuo das condições climáticas em tempo real.

2. Será possível fazer previsões confiáveis, pois será feita uma análise de dados combinada com o Machine Learning e isso possibilitará uma previsão precisa sobre os desastres naturais.

3. Redução do impacto dos desastres naturais, Ao fornecer previsões confiáveis e alertas antecipados, esperamos reduzir os impactos causados pelos desastres naturais pois a população e governo terá as informações previamente e assim poderá tomar medidas cautelares como evacuações de cidades para reduzir o impacto humanitário e até mesmo financeiro.

4. Velocidade do alerta, assim que aprovado pelos especialistas as informações devem ser compartilhadas rapidamente para que seja possível disseminar o alerta para o maior número de pessoas em menor espaço de tempo possível

5. Apoio a decisões governamentais e de gestão: O sistema irá fornecer informações sólidas para especialistas e autoridades competentes para que as mesma temem decisões mais rápidas e embasadas com dados reais. facilitando assim a gestão de desastres naturais  

# 10. Conclusão

Levando em consideração a frequência e intensidade de desastres naturais, tanto no Brasil como no mundo, como por exemplo as inundações do Rio Grande do Sul mais especificamente nas cidades Eldorado do sul, Muçum e Canoas onde a população sofreu perdas econômicas e sociais de até 81%, torna-se necessário o desenvolvimento de soluções tecnológicas, que realizam a previsão e monitoramento para que seja possível mitigar os impactos causados por esses eventos. Com a  utilização de dados que foram extraídos do IOT pelo INMET como base para a análise de ML e IA, para validar os dados será utilizado ITS para que seja possível a criação de um sistema autônomo e inteligente para previsão de desastres
Após a validação realizada pelo ITS, geralmente é realizado um tratamento dos dados para que assim seja possível utilizarem a lógica FUZZY para tratar dados incertos e complexos, auxiliando para uma análise mais precisa e realista dos cenários climáticos. Para o desenvolvimento da análise dos dados serão testados os seguintes modelos híbridos de ensemble: Random Forest, Boosted Regression Trees e Extremely Randomized Trees, com o objetivo de otimizar a predição de enchentes, considerando variáveis ambientais e geográficas fundamentais.
Por fim, seria enviado um alerta a um centro de mitigação de risco contendo especialistas na área que validarão e somente após a aprovação será enviado um alerta a região através de Smart Alarm e um post nas redes sociais informando sobre o acontecimento para que seja possível atingir a maior quantidade de pessoas em um curto espaço de tempo.
Pode-se concluir que, o projeto não possui apenas como objetivo reduzir perdas humanas e materiais, mas criar uma ferramenta capaz de auxiliar autoridades, gestores e especialistas para tomada de decisão que irá proteger a população em geral. O mesmo irá enfrentar de forma proativa os desafios e perigos criados pelas mudanças climáticas gerando assim um futuro mais seguro, sereno, resiliente e sustentável.
 
# 10. Referências
 
ABDELWAHAB, M. ABO-ZAHHAD, M. ABRAHAM, K. Classification and detection of natural disasters using machine learning and deep learning techniques: A review. Earth Sci Inform. Egito. v.17. n 1. p 869–891 (2024). https://doi.org/10.1007/s12145-023-01205-2
ADALZAHER, MOHAMED S; ELSAYED, HUSSEIN A; FOUDA, MOSTAFA, M; Employing Remote Sensing, Data Communication Networks, AI, and Optimization Methodologies in Seismology. IEEE JOURNAL OF SELECTED TOPICS IN APPLIED EARTH OBSERVATIONS AND REMOTE SENSING. [S.L.]. v. 15. n. 9417. p.9417 - 9438.Outubro 2022.
ADI K. GERNOWO, R. USMAN, C, D. WIDODO, A, P. Rainfall prediction model in Semarang City using machine learning, Indonesian Journal of Electrical Engineering and Computer Science. Indonésia. v.30, n. 2, p. 1224-1231 Maio 2023.
ALASKAR H; AL-JUMEILY D; BAKER T; BUYYA R; HUSSAIN A. J; KHALAF M; KHAN W; LIATSIS P; MAAMAR Z; TAWFIK H. IoT-Enabled Flood Severity Prediction via Ensemble Machine Learning Models. IEEE JOURNAL OF SELECTED TOPICS IN APPLIED EARTH OBSERVATIONS AND REMOTE SENSING. v. 8, p. 70375-70386. Abril 2020
ALHAMIDI; PAKPAHAN, V.H; SIMANJUNTAK, J. E. S. Analysis of tsunami disaster resilience in Bandar Lampung Bay Coastal Zone. IOP Conference Series: Earth and Environmental Science. Indonésia. v. 158. n.012037. p 1-10. Novembro 2024.
AMAJUOYI, BRIGHT C; ARTHUR, JOACHIM KODJO; HOSSEINIAN-FAR, AMIN; NJOKU; OGUGUO C; SARWAR, DILSHAD. Impact of an Integrated Approach in Disaster Management. International Journal of Organizational and Collective Intelligence. Reino Unido. [S.L]. v. 10. n. 2. p 20-36. Abril/Junho 2020.
AMITRANO D; DI MARTINO G; DI SIMONE A; IMPERATORE P. Flood Detection with SAR: A Review of Techniques and Datasets. Remote Sens. v.16, n.4, p.656-694. Fevereiro 2024
ANGRIAWAN, RANDY; ARIF, YUNIFA MIFTACHUL; H, MUHAMMAD, RIZAL; HARIADI, MOCHAMAD; MAULINA, DINA; WARNI, ELLY. Design of Flood Early Detection Based on the Internet of Things and Decision Support System. International Information and Engineering Tecnology Association. Indonésia. v. 19. n. 3. p 1183-1193. Junho 2024.
ASIF, MD; COLAK, ILHAMI; NUVVULA, RAMAKRISHNA S. S; KHAN, BASEEM; KUMAR, POLAMARASETTY P; KRISHNAMOORTHY, MURUGAPERUMAL. A Design and Development of the Smart Forest Alert Monitoring System Using IoT. Journal of Sensors. [S.L]. v. 2023. n. 1. Setembro 2022/Fevereiro 2023.
BAND, S. S.; JANIZADEH, S.; CHANDRA PAL, S.; SAHA, A.; CHAKRABORTTY, R.; MELESSE, A.M.; MOSAVI, A. Flash Flood Susceptibility Modeling Using New Approaches of Hybrid and Ensemble Tree-Based Machine Learning Algorithms. Remote Sens. 2020, v.12, n. 21 p 3568 - 3591.
DELAVAR M. R; HABIBI A; NAZARI B; PIRASTEH S; SADEGHIAN M. S. A hybrid of ensemble machine learning models with RFE and Boruta wrapper-based algorithms for flash flood susceptibility assessment. Iran, v.122, n.6, p. 69 – 87, Junho 2023.
DUC, D. N. M.; KHOA, C. N. D.; KHOA, T. A.; MINH, N. Q.; NAM, N. H.; SON, H. H.; TAN, D. N.; TIN, N. T.; VANDUNG, N. Wireless sensor networks and machine learning meet climate change prediction. International Journal of Communication Systems. [S.L] v. 34; n. e4687. Novembro 2020.
G1. Um mês de enchentes no RS: veja cronologia do desastre que atingiu 471 cidades, matou mais de 170 pessoas e expulsou 600 mil de casa.  29/05/2024. Disponível em: https://g1.globo.com/rs/rio-grande-do-sul/noticia/2024/05/29/um-mes-de-enchentes-no-rs-veja-cronologia-do-desastre.ghtml. Acesso em: 16/05/2025
HANS, M. R.; HAZRA, N.; RAJ, A. IoT Based Flood Monitoring and Alerting System. International Journal for Research in Applied Science & Engineering Technology (IJRASET). India. v.12. n.2. Fevereiro 2024.
GHANSHALA, K., K.; GOYAL, H. R.; SHARMA, S. Role of IoT devices in Flood Monitoring System using Social Networking Sites. International Journal of Innovative Technology and Exploring Engineering (IJITEE). India. v. 9. n. 4. Fevereiro 2024.
INSTITUTO DE PESQUISA ECONÔMICA APLICADA (IPEA). 876 mil pessoas foram diretamente atingidas pelas enchentes no Rio Grande do Sul. In: Acompanhe o IPEA – Noticias. 17/07/2024. Disponível em: https://www.ipea.gov.br/portal/categorias/45-todas-as-noticias/noticias/15183-876-mil-pessoas-foram-diretamente-atingidas-pelas-enchentes-no-rio-grande-do-sul#:~:text=876%20mil%20pessoas%20foram%20diretamente%20atingidas%20pelas%20enchentes%20no%20Rio%20Grande%20do%20Sul-Estimativa%20do%20Ipea. Acesso em: 20 out. 2024.
INSTITUTO NACIONAL DE METEOROLOGIA (INMET). DADOS HISTÓRICOS ANUAIS. 01/01/2025. Disponível em: https://portal.inmet.gov.br/dadoshistoricos. Acesso em: 16/05/2025
KAVAK, A; KHAN, S, A; SADEQ, A. S. A Data Transmission Scheme Using K-Means and Fuzzy Logic for IOT Sensor Based Forest Fire Detection System. International Journal of Emerging Trends in Engineering Research, Turkia. v. 10. n. 10, p1-5, Setembro/Outubro, 2022.
PATSAVELLAS, J.; KAUR, R.; SALONITIS, K. Supply chain control towers: Technology push or marketpull—An assessment tool. IET Collaborative Intelligent Manufacturing. Reino Unido. v. 3. n. 3. p 290-302. Setembro 2021.
SADANANDAN, S, K; SARKER, P, S; SRIVASTAVA, A, K. Resiliency Metrics for Monitoring and Analysis of Cyber-Power Distribution System with IoTs. IEEE Internet of Things Journal. Estados Unidos. v. 10. n. 9. p 7469 - 7479, Dezembro, 
