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
 
O projeto surge para enfrentar os desafios impostos pela natureza por meio de desastres naturais mais especificamente inundações como por exemplo a inundação do Rio Grande do Sul onde 876 mil pessoas foram afetadas negativamente perdendo suas casas, animais de estimação e muitas vezes até suas vidas por causa da inundação ocorrida no dia 27 de abril de 2024 (IPEA, 2024). Portanto o projeto propõe utilizar os dados da internet das coisas (Internet of things, IOT) (PATSAVELLAS,2021) juntamente com técnicas de aprendizado de máquina (Machine Learning, ML) (DUC, 2020) para que seja possível construir uma solução de monitoramento, previsão e até mesmo divulgação de alertas em tempo real. Essa abordagem visa gerar e transmitir dados precisos e relevantes para auxiliar a tomada de decisão de equipes e entidades competentes. A solução irá utilizar sensores IOT distribuídos de forma estratégica para que seja possível a captação de informações ambientais como nível de chuva, umidade do solo e velocidade do vento. Esses dados serão processados por algoritmos de ML que será utilizado como base para uma Inteligência Artificial (Artificial Inteligence, IA) treinada que será responsável pela identificação de padrões que precedem eventos climáticos extremos. Com base nos dados analisados, o sistema irá gerar previsões de inundações, outros desastres associados e as áreas que serão mais afetadas. Como consequência, irá oferecer insights sobre a possibilidade e a gravidade desses eventos em locais específicos. Para garantir a confiabilidade e a integridade dessas informações, os dados que serão obtidos passaram por uma avaliação de pontuação de confiabilidade (IoT Trustability Score, ITS) (SADANANDAN, 2021). Essa avaliação irá verificar a consistência e a precisão dos dados fornecidos pelos sensores, integrando assim uma rede neural que identificará e filtrará possíveis inconsistências. Com isso, será possível aumentar a confiabilidade dos alertas emitidos. Os dados são convertidos em gráficos e indicadores visuais utilizando a Lógico Fuzzy (ADALZAHER, 2022), que permitirá o processamento de informações incertas e auxiliará na interpretação dos resultados. Em seguida, especialistas irão validar as informações processadas e aprovarão, ou não, a divulgação dos alertas. A comunicação dos resultados irá ocorrer por meio das redes sociais, outras plataformas digitais e até mesmo alarmes inteligentes (Smart alarms) (ASIF, 2023), com o objetivo de alcançar rapidamente o maior número de pessoas e permitir assim que a população e o governo tomem as medidas necessárias para segurança pessoal e coletiva. O sistema que foi proposto busca otimizar a resposta a desastres naturais e reduzir os impactos, proporcionando assim uma ferramenta poderosa de apoio à decisão para gestores e autoridades competentes envolvidas no gerenciamento de crises ambientais.
 
# 5.   	Descrição do Problema

O problema enfrentado é a falta de resposta eficiente em um tempo hábil e isso causava uma inevidência no combate aos desastres naturais, especialmente nas inundações. Esse acontecimento pode ser observado com mais clareza nas inundações do Rio Grande do Sul do dia 27 de abril de 2024. Os efeitos dessas catástrofes foram devastadoras pois tiveram muitas perdas de vidas humanas e não humanas, perda de moradias, perda de muitos investimentos que tinha na cidade e etc. Dito isso, o projeto tem como foco a incapacidade de prever com velocidade e precisão esses eventos, o que acarreta em uma perdas inestimáveis. hoje em dia a previsão de desastres naturais depende métodos mais arcaicos que não são tão eficazes por se tratar de um complexo entendimento dos dados da natureza. a falta de um sistema integrado com as redes sociais e um sistema que gera dados em gráficos de fácil leitura para especialistas acarreta em uma gestão de desastres naturais ineficiente e demorada. Portanto o projeto enfrenta um desafio em criar uma solução tecnológica que integre o monitoramento em tempo real, previsão de eventos externos e uma comunicação rápida e eficiente de alertas para toda população. 
# 6. Aspectos Éticos


Um dos aspectos importantes é o armazenamento de dados sensíveis, como o endereço do usuário por ser uma parte crucial do sistema. Os dados serão criptografados e armazenados em um banco de dados separados, e o acesso aos dados será restrito dentro do sistema para garantir a confidencialidade dos usuários. Para o tratamento de dados, os dados só serão utilizados para decidir qual será a área da comunicação de acordo com os dados meteorológicos presentes no sistema.
A IA será utilizada na questão de análise de dados, onde as chuvas serão analisadas ao longo do tempo para poder gerar a previsão do próximo 

# 7. Dataset

Nossa base de dados contém uma coluna que se refere à data, outra coluna com os horários do dia, espaçados em períodos de 1 hora cada, uma coluna dizendo a quantidade de precipitação em milímetros naquele momento, e por fim, temos 3 colunas dizendo a umidade relativa do ar média, mínima e máxima, em porcentagem.

# 8.   	Metodologia e Resultados Esperados
 
Metodologia
O projeto busca integrar informações fornecidas pelo Iot para treinar um aprendizado de máquina para que seja possível desenvolver uma solução robusta e eficaz no monitoramento e previsão de inundações e outros desastres naturais. A metodologia é composta por:

1. Será usado dados de Iot já preexistentes, portanto será utilizado um dataset já previamente definido.

2. Processamento e análise de dados com Machine Learning, após obtenção dos dados eles serão processados por um algoritmo de aprendizado da máquina. A análise dos dados será conduzida por uma Inteligência Artificial que será treinada para identificar padrões climáticos que geralmente migram para desastres naturais. Portanto, a IA será responsável por gerar previsões sobre a possibilidade e a gravidade dos eventos, além de identificar as áreas mais afetadas.

3. Será utilizado a Lógica Fuzzy para processar as incertezas, levando em consideração incerteza sobre a natureza e a grande variação de dados ambientais, será empregada a Lógica Fuzzy para transformar informações em gráficos. Facilitando assim, a criação de indicadores visuais de fácil visualização e interpretação.

4. Validação e divulgação dos alertas, os resultados serão avaliados por especialistas no centro de mitigação, que revisarão as previsões antes de sua divulgação. Caso os especialistas aprovem os dados, será feito a divulgação para a população por meio de redes sociais e alarmes inteligentes, garantindo assim que a informação chegue rapidamente a população. 

Resultados esperados

1. Irá permitir um monitoramento de uma cidade, estado ou até mesmo país em tempo real, pois com a implementação do sistema será possível um monitoramento contínuo das condições climáticas em tempo real.

2. Será possível fazer previsões confiáveis, pois será feita uma análise de dados combinada com o Machine Learning e isso possibilitará uma previsão precisa sobre os desastres naturais.

3. Redução do impacto dos desastres naturais, Ao fornecer previsões confiáveis e alertas antecipados, esperamos reduzir os impactos causados pelos desastres naturais pois a população e governo terá as informações previamente e assim poderá tomar medidas cautelares como evacuações de cidades para reduzir o impacto humanitário e até mesmo financeiro.

4. Velocidade do alerta, assim que aprovado pelos especialistas as informações devem ser compartilhadas rapidamente para que seja possível disseminar o alerta para o maior número de pessoas em menor espaço de tempo possível

5. Apoio a decisões governamentais e de gestão: O sistema irá fornecer informações sólidas para especialistas e autoridades competentes para que as mesma temem decisões mais rápidas e embasadas com dados reais. facilitando assim a gestão de desastres naturais  

# 9. REFERENCIAL TEÓRICO 

O surgimento da IOT (PATSAVELLAS,2021) se deu a partir da quarta revolução industrial (4º Industrial Revolution 4IR), que permitiu o avanço da conexão sem fio e a conexão entre os mundos digital, biológicos e físicos, tornando assim possível a conexão entre dispositivos eletrônicos. (ANGRIAWAN, 2024)
A crescente necessidade de utilizar diversos sensores em aplicações de IoT impulsionou o desenvolvimento das redes de sensores sem fio (Wireless Sensor Network, WSN). Essas redes possibilitam que múltiplos sensores se conectem a um cluster, responsável pelo processamento inicial das informações antes de enviá-las ao Arduino, onde são aplicadas

condições predefinidas para a tomada de decisões (KAVAK, 2022). Esse processo permite a integração de vários sensores ao cluster, viabilizando o processamento prévio de grandes volumes de dados, que são então enviados ao Arduino.
Esses dados, ao serem processados, podem alimentar algoritmos de ML para diversas finalidades (DUC, 2020), incluindo a aplicação de IA em previsões, como a mitigação de desastres naturais a partir de dados coletados. Com os dados de entrada processados pela IA, são geradas previsões futuras; entretanto, devido à incerteza inerente, torna-se necessária a aplicação da lógica Fuzzy, que trata esses dados incertos e os torna mais regulares (ADALZAHER, 2022).
Porém, mesmo após esse tratamento, os dados podem apresentar limitações de confiabilidade, o que demanda a aplicação do ITS (SADANANDAN, 2021). Essa tecnologia permite que uma rede neural aprenda e valide o nível de confiabilidade dos dados fornecidos, oferecendo uma camada adicional de segurança e precisão aos dados processados, a demanda de verificação da confiabilidade dos dados a partir do ITS se faz necessário pois serão analisados dados de previsão de desastres naturais.
Por fim, após a validação do ITS os dados serão analisados por um grupo de especialistas que validarão, ou não, o envio do alerta para a região afetada. Esse alerta será feito de 2 formas: a primeira soará um Smart alarm (ASIF, 2023) que avisará a população instalada na região para se retirar do local. Em seguida será realizado um post nas redes sociais dentro de 10 minutos informando o motivo do alarme, o que permitirá que pessoas de todo o mundo saiba da situação e possa ajudar nesse momento de fragilidade da região.
Para a mitigação de desastres naturais, o uso de tecnologias como IoT, WSN e a lógica Fuzzy permite obter dados em tempo real de múltiplos sensores conectados a servidores. Essas informações facilitam análises que permitem decisões mais assertivas, como a previsão e resposta a uma possível inundação. Com a coleta e análise desses dados, é possível criar uma base sólida para um sistema de alerta e resposta eficiente.
 
 
# 10. Bibliografia
 
ADALZAHER, Mohamed S; ELSAYED, Hussein A.; FOUDA, Mostafa, M.; Employing Remote Sensing, Data Communication Networks, AI, and Optimization Methodologies in Seismology. IEEE JOURNAL OF SELECTED TOPICS IN APPLIED EARTH OBSERVATIONS AND REMOTE SENSING. [S.L.]. v. 15. n. 9417. p.9417 - 9438.
Outubro 2022.
ALHAMIDI; PAKPAHAN, V.H; SIMANJUNTAK, J. E. S. Analysis of tsunami disaster resilience in Bandar Lampung Bay Coastal Zone. IOP Conference Series: Earth and Environmental Science. Indonésia. v. 158. n.012037. p 1-10. Novembro 2024.
AMAJUOYI, Bright C; ARTHUR, Joachim Kodjo; HOSSEINIAN-FAR, Amin; NJOKU,
Oguguo C; SARWAR, Dilshad. Impact of an Integrated Approach in Disaster Management. International Journal of Organizational and Collective Intelligence. [S.L].
v. 10. n. 2. p 20-36. Abril/Junho 2020.
ANGRIAWAN, Randy; ARIF, Yunifa Miftachul; H, Muhammad, Rizal; HARIADI, Mochamad; MAULINA, Dina; WARNI, Elly. Design of Flood Early Detection Based on the Internet of Things and Decision Support System. International Information and Engineering Tecnology Association. Indonésia. v. 19. n. 3. p 1183-1193. Junho 2024.
ASIF, Md; COLAK, Ilhami; NUVVULA, Ramakrishna S. S; KHAN, Baseem; KUMAR, Polamarasetty P; KRISHNAMOORTHY, Murugaperumal. A Design and Development

of the Smart Forest Alert Monitoring System Using IoT. Journal of Sensors. [S.L]. v. 2023. n. 1. Setembro 2022/Fevereiro 2023.
DUC, Dang Ngoc Minh; KHOA, Cao Nguyen Dang; KHOA, Tran Ahn; MINH, Nguyen Quang; NAM, Nguyen Hoang; SON, Hoang Hai; TAN, Dinh Ngoc; TIN, Nguyen Trung; VANDUNG, Nguyen. Wireless sensor networks and machine learning meet climate change prediction. International Journal of Communication Systems. [S.L] v. 34; n. e4687. Novembro 2020.
CHAVAN, Prajakta; PABALKAR, Vaishnavi; SALUNKE, Divya; TAUARI, Nalini; KHAIRNAR, Prajakata. IoT Based Flood Monitoring and Alerting System. International Journal for Research in Applied Science & Engineering Technology (IJRASET). India. v.
12. n.2. Fevereiro 2024.
GHANSHALA, Kamail, Kumar; GOYAL, Himanshu, Rai. Role of IoT devices in Flood Monitoring System using Social Networking Sites. International Journal of Innovative Technology and Exploring Engineering (IJITEE). India. v. 9. n. 4. Fevereiro 2024.
INSTITUTO DE PESQUISA ECONÔMICA APLICADA (IPEA). 876 mil pessoas foram
diretamente atingidas pelas enchentes no Rio Grande do Sul. In: Acompanhe o IPEA – Noticias. 17/07/2024. Disponível em: https://www.ipea.gov.br/portal/categorias/45- todas-as-noticias/noticias/15183-876-mil-pessoas-foram-diretamente-atingidas-pelas- enchentes-no-rio-grande-do-sul#:~:text=876%20mil%20pessoas%20foram%20 diretamente%20atingidas%20pelas%20enchentes%20no%20Rio%20Grande%20do%20 Sul,-Estimativa%20do%20Ipea. Acesso em: 20 out. 2024.
KAVAK, A; KHAN, S, A; SADEQ, A. S. A Data Transmission Scheme Using K-Means and Fuzzy Logic for IOT Sensor Based Forest Fire Detection System. International Journal of Emerging Trends in Engineering Research, Turkia. v. 10. n. 10, p1-5, Setembro/Outubro, 2022.
PATSAVELLAS, John; KAUR, Rashmeet; SALONITIS, Konstatinos. Supply chain control towers: Technology push or marketpull—An assessment tool. IET Collaborative Intelligent Manufacturing. Reino Unido. v. 3. n. 3. p 290-302. Setembro 2021.
SADANANDAN, S, K; SARKER, P, S; SRIVASTAVA, A, K. Resiliency Metrics for
Monitoring and Analysis of Cyber-Power Distribution System with IoTs. IEEE Internet of Things Journal. Estados Unidos. v. 10. n. 9. p 7469 - 7479, Dezembro, 2021.
