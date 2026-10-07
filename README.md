# pericia
Projeto acadêmico da disciplina de Projeto Integrador em Perícia Computacional.
## 1.1 Objetivo Geral

Analisar uma evidência digital no contexto da computação forense, utilizando procedimentos técnicos de identificação, coleta, aquisição, preservação e análise de dados, com o objetivo de compreender os acontecimentos relacionados ao uso da máquina virtual investigada e garantir a integridade, autenticidade e rastreabilidade das informações obtidas durante o processo pericial.

---

## 1.2 Objetivos Específicos

Para alcançar o objetivo geral proposto, estabelecem-se os seguintes objetivos específicos:

- **Conceituar** a evidência digital e a computação forense, apresentando seus principais fundamentos e sua importância no contexto das investigações digitais;
- **Identificar** as principais fontes de evidência digital presentes na máquina virtual investigada, considerando arquivos, diretórios, sistemas de arquivos, registros do sistema, metadados, usuários, aplicações e demais informações relevantes;
- **Examinar** as características dos dados digitais encontrados, considerando aspectos como alteração, exclusão, sobrescrita, reprodução e volatilidade das informações;
- **Aplicar** procedimentos de identificação e aquisição da evidência digital, utilizando métodos que reduzam o risco de alteração ou perda dos dados durante o processo investigativo;
- **Preservar** a evidência digital obtida, utilizando mecanismos de controle de integridade, como funções de hash, e registrando as informações necessárias para garantir sua rastreabilidade durante as etapas da perícia;
- **Documentar** a cadeia de custódia da evidência digital, registrando as etapas de identificação, coleta, aquisição, armazenamento, processamento e análise, bem como os responsáveis e procedimentos realizados em cada etapa;
- **Analisar** os dados obtidos da máquina virtual, considerando arquivos, registros de sistema, metadados, histórico de atividades, informações de usuários, aplicações e outros artefatos digitais relevantes para a investigação;
- **Correlacionar** diferentes artefatos e fontes de evidência encontrados durante a análise, buscando estabelecer relações entre usuários, arquivos, dispositivos, atividades e eventos para auxiliar na reconstrução dos acontecimentos;
- **Verificar** a confiabilidade dos resultados obtidos por meio da comparação dos valores de hash, da análise dos registros da cadeia de custódia, da preservação dos dados originais e da documentação dos procedimentos realizados;
- **Avaliar** a contribuição das evidências encontradas para a reconstrução dos acontecimentos investigados, considerando a consistência das informações, a relação temporal entre os eventos e a possibilidade de confirmar os fatos por meio de diferentes artefatos digitais.

---

## 1.3 Justificativa

O avanço das tecnologias digitais e a ampliação do uso de dispositivos eletrônicos modificaram significativamente a forma como as informações são produzidas, armazenadas e compartilhadas. Computadores, smartphones, servidores, redes de comunicação e sistemas informatizados passaram a fazer parte de atividades pessoais, profissionais e institucionais. Como consequência, uma quantidade cada vez maior de informações é registrada em meios digitais, tornando esses dados relevantes para a apuração de fatos e para diferentes tipos de investigação.

Nesse contexto, a evidência digital apresenta papel importante na computação forense, pois arquivos, registros de sistemas, mensagens, dados de navegação, informações de acesso, metadados e outros artefatos podem fornecer informações relacionadas à ocorrência de determinado fato. Entretanto, diferentemente de evidências físicas tradicionais, os dados digitais podem ser facilmente alterados, excluídos, sobrescritos ou modificados, inclusive durante sua própria coleta e análise. Essa característica exige a adoção de procedimentos técnicos capazes de reduzir a possibilidade de alterações e preservar as características originais das informações.

A ISO/IEC 27037:2012 estabelece diretrizes para a identificação, coleta, aquisição e preservação de potenciais evidências digitais, servindo como uma importante referência para o tratamento inicial desses vestígios. A norma destaca a necessidade de procedimentos controlados para reduzir riscos de alteração e preservar a utilidade da evidência durante o processo investigativo. Além disso, a ISO/IEC 27042:2015 apresenta orientações relacionadas à análise e interpretação das evidências digitais, considerando aspectos como validade, continuidade, reprodutibilidade e possibilidade de verificação dos procedimentos realizados.

Outro aspecto fundamental é a rastreabilidade da evidência. O registro das etapas de identificação, coleta, aquisição, armazenamento, processamento e análise permite acompanhar o tratamento realizado e documentar as intervenções efetuadas sobre os dados. Dessa forma, a preservação e a cadeia de custódia não são consideradas apenas etapas isoladas, mas elementos que contribuem para demonstrar a integridade e a confiabilidade do material analisado ao longo da investigação.

Apesar da existência de normas e procedimentos voltados ao tratamento da evidência digital, a aplicação prática desses conceitos pode apresentar dificuldades, principalmente quando é necessário relacionar os procedimentos técnicos à análise dos artefatos efetivamente encontrados em um ambiente computacional. Nesse sentido, este estudo busca abordar essa lacuna por meio da aplicação prática de procedimentos de computação forense em uma máquina virtual, permitindo relacionar os fundamentos teóricos da evidência digital com as etapas de identificação, aquisição, preservação, documentação e análise dos dados encontrados.

A delimitação do estudo em uma máquina virtual permite concentrar a investigação nos principais artefatos disponíveis nesse ambiente, como arquivos, registros do sistema, informações de usuários, metadados e históricos de atividades. A partir desses elementos, pretende-se demonstrar como diferentes evidências podem ser analisadas e correlacionadas para auxiliar na compreensão e reconstrução dos acontecimentos observados.

A realização do estudo também apresenta relevância acadêmica por integrar conhecimentos de computação forense, segurança da informação, sistemas operacionais e análise de dados. A aplicação prática dos procedimentos permite compreender não apenas os conceitos relacionados à evidência digital, mas também os cuidados necessários para que os resultados obtidos sejam documentados, rastreáveis e passíveis de verificação.

Dessa forma, a pesquisa justifica-se pela necessidade de compreender, de maneira teórica e prática, como evidências digitais podem ser identificadas, adquiridas, preservadas e analisadas em um ambiente computacional controlado. Ao relacionar os procedimentos técnicos com os artefatos encontrados na máquina virtual investigada, o estudo busca contribuir para uma compreensão mais consistente do processo de tratamento da evidência digital e dos fatores que influenciam sua integridade, rastreabilidade e confiabilidade.
# 2. Referencial Teórico

## 2.1 Evidência Digital: Conceito e Características

A utilização de tecnologias digitais nas atividades sociais, profissionais e institucionais modificou significativamente os processos de produção, armazenamento e transmissão de informações. Nesse contexto, computadores, dispositivos móveis, redes e sistemas informatizados passaram a constituir importantes fontes de dados para atividades investigativas. A evidência digital, nesse cenário, apresenta relevância para a apuração de fatos e para a reconstrução de acontecimentos relacionados a determinada investigação.

A evidência digital pode ser compreendida como informação armazenada ou transmitida em formato digital que apresenta relevância para uma investigação. Pollitt (2009) relaciona a evidência digital às informações obtidas a partir de sistemas e dispositivos digitais que podem contribuir para a compreensão de fatos investigados. Casey (2011), por sua vez, observa que os vestígios digitais podem estar presentes em diferentes dispositivos e sistemas tecnológicos, fornecendo informações relacionadas a atividades realizadas, acontecimentos e relações entre diferentes elementos de uma investigação.

Computadores, redes e demais dispositivos digitais constituem, portanto, fontes de informações que podem contribuir para o esclarecimento de determinados fatos. O National Institute of Standards and Technology (NIST) aborda a perícia digital como um processo relacionado à identificação, aquisição, preservação e análise de dados eletrônicos que possam apresentar relevância para uma investigação. Sob essa perspectiva, a evidência digital não corresponde apenas a uma informação isolada, mas integra um conjunto de procedimentos destinados à obtenção e ao tratamento dos dados.

A natureza da evidência digital apresenta características particulares quando comparada às evidências físicas. Os dados podem ser copiados, modificados, excluídos ou sobrescritos sem que essas alterações sejam necessariamente perceptíveis. Essa característica exige procedimentos específicos para o tratamento dos vestígios digitais, especialmente no que se refere à preservação da integridade das informações e à possibilidade de verificação dos procedimentos realizados.

---

## 2.2 Fontes de Evidência Digital

As evidências digitais podem ser encontradas em diferentes dispositivos, sistemas e ambientes tecnológicos. Computadores, servidores, dispositivos móveis, mídias de armazenamento, redes, aplicativos e serviços digitais podem armazenar ou produzir informações relevantes para uma investigação.

Carrier (2005) destaca a importância dos sistemas de arquivos para a análise forense computacional. O conhecimento de sua estrutura permite identificar arquivos, diretórios, metadados e outras informações relacionadas ao armazenamento dos dados. Dependendo das características do dispositivo e do sistema analisado, também podem ser obtidas informações relacionadas a arquivos excluídos.

Casey (2011) apresenta diferentes fontes de evidência presentes em computadores, redes e outros dispositivos, incluindo arquivos, registros de sistema, informações de navegação, mensagens eletrônicas e dados relacionados ao uso de aplicações. A análise desses elementos pode fornecer informações relevantes para a compreensão dos acontecimentos investigados.

O NIST SP 800-86 considera diferentes categorias de dados que podem ser utilizadas em investigações forenses, abrangendo informações provenientes de arquivos, sistemas operacionais, redes e aplicações. A análise dessas fontes permite estabelecer relações entre diferentes informações e ampliar a compreensão sobre determinado acontecimento.

A identificação das fontes de evidência constitui, assim, uma etapa relevante da investigação digital. Dados provenientes de diferentes dispositivos ou sistemas podem apresentar relação entre si e, quando analisados conjuntamente, contribuir para a reconstrução dos fatos.

---

## 2.3 Identificação, Coleta e Aquisição da Evidência Digital

A identificação, a coleta e a aquisição constituem etapas fundamentais no tratamento da evidência digital. A interação com um dispositivo durante uma investigação pode modificar ou eliminar determinados dados, sobretudo quando se trata de informações sujeitas a alterações constantes. Por esse motivo, os procedimentos empregados devem ser realizados de forma controlada e devidamente documentada.

A ISO/IEC 27037:2012 estabelece orientações para a identificação, coleta, aquisição e preservação de evidências digitais. A norma apresenta procedimentos destinados ao tratamento de potenciais evidências digitais, contribuindo para a manutenção das informações durante as etapas iniciais da investigação.

Casey (2011) apresenta a investigação digital como um processo que envolve atividades relacionadas à identificação, preservação, recuperação e análise das informações. A utilização de procedimentos organizados reduz a possibilidade de alterações indevidas e permite acompanhar as etapas realizadas durante o tratamento da evidência.

Kent et al. (2006), por meio do NIST SP 800-86, apresentam um processo estruturado para a aplicação de técnicas forenses no contexto da resposta a incidentes. Entre as atividades descritas encontram-se a identificação e aquisição dos dados, a proteção das informações coletadas, o processamento, a análise e a apresentação dos resultados.

A coleta e a aquisição da evidência digital devem ser realizadas de maneira controlada, buscando minimizar alterações nos dados originais. A documentação das ações executadas também constitui parte relevante desse processo, uma vez que permite registrar as intervenções realizadas e possibilita a posterior verificação dos procedimentos empregados.

---

## 2.4 Preservação, Integridade e Cadeia de Custódia

A preservação da evidência digital é necessária diante da possibilidade de alteração, corrupção ou perda dos dados durante o processo investigativo. Seu objetivo consiste em manter as características das informações obtidas e possibilitar a verificação dos procedimentos realizados durante seu tratamento.

Guttman et al. (2022) destacam que a preservação de evidências digitais apresenta dificuldades específicas relacionadas à diversidade de dispositivos, sistemas e objetos digitais. A adoção de procedimentos apropriados é necessária para manter as informações disponíveis e preservar suas características ao longo das diferentes etapas do processo.

A ISO/IEC 27037:2012 inclui a preservação entre as atividades relacionadas ao tratamento da evidência digital, juntamente com a identificação, coleta e aquisição. A aplicação de procedimentos definidos contribui para reduzir o risco de alterações durante a manipulação dos dados.

Casey (2011) também destaca a importância da documentação dos procedimentos realizados durante a investigação. O registro das ações permite acompanhar o tratamento da evidência desde sua obtenção até as etapas de análise e apresentação dos resultados.

Nesse contexto, a cadeia de custódia corresponde ao registro do histórico da evidência desde sua identificação e coleta até seu armazenamento, processamento e análise. A documentação desse percurso permite acompanhar as intervenções realizadas sobre o material e verificar as condições em que a evidência foi mantida durante o processo investigativo.

---

## 2.5 Análise e Interpretação da Evidência Digital

Após a identificação, aquisição e preservação, os dados coletados são submetidos à análise com o objetivo de localizar informações relevantes para a investigação. Essa etapa exige conhecimentos relacionados aos dispositivos, sistemas operacionais, sistemas de arquivos, redes e aplicações.

Carrier (2005) demonstra que a análise dos sistemas de arquivos permite identificar diferentes estruturas e informações relacionadas ao armazenamento dos dados. Arquivos, diretórios, metadados e outros elementos podem fornecer informações relevantes para a investigação e auxiliar na compreensão da organização dos dados armazenados.

Casey (2011) destaca que a análise forense não se limita à localização de informações isoladas. A comparação e a correlação entre diferentes elementos podem contribuir para estabelecer relações entre acontecimentos e reconstruir a sequência de determinadas atividades.

O NIST SP 800-86 apresenta a análise de diferentes fontes de dados, incluindo arquivos, sistemas operacionais, tráfego de rede e aplicações. A utilização dessas informações possibilita estabelecer relações entre os diferentes elementos identificados durante a investigação.

A interpretação dos dados deve considerar sua origem, contexto, características técnicas e relação com outras informações obtidas. Dessa maneira, a análise ultrapassa a simples identificação de determinado dado e busca compreender sua relevância em relação aos acontecimentos investigados.

---

## 2.6 Evidência Digital em Investigações Forenses

A utilização de dispositivos e serviços digitais nas atividades cotidianas tornou os registros eletrônicos relevantes para diferentes modalidades de investigação. Informações armazenadas em computadores, dispositivos móveis, redes e sistemas podem fornecer dados relacionados a usuários, horários, atividades, dispositivos e conexões.

Casey (2011) demonstra que computadores e redes podem constituir tanto instrumentos utilizados na realização de determinadas atividades quanto fontes de informações para sua investigação. A análise dos registros digitais pode auxiliar no estabelecimento de relações entre pessoas, dispositivos e acontecimentos.

Pollitt (2009) relaciona a perícia digital à identificação e interpretação de informações relevantes para uma investigação. Nesse contexto, os dados devem ser analisados considerando sua origem e sua relação com os demais elementos disponíveis.

O NIST SP 800-86 apresenta a utilização de técnicas forenses na investigação de incidentes e considera diferentes fontes de informação no processo de identificação, aquisição, processamento, análise e apresentação dos resultados.

A evidência digital pode contribuir para a investigação de diferentes acontecimentos, desde que sua obtenção, preservação, análise e documentação sejam realizadas de acordo com procedimentos técnicos apropriados. A observância dessas etapas possibilita maior controle sobre as informações utilizadas durante o processo investigativo e contribui para a confiabilidade dos resultados obtidos.

---

## 2.7 Síntese do Referencial Teórico

A evidência digital constitui uma importante fonte de informações para investigações, especialmente diante da crescente utilização de dispositivos e sistemas tecnológicos. As características próprias dos dados digitais exigem procedimentos específicos relacionados à identificação, coleta, aquisição, preservação e análise.

Os estudos de Casey (2011), Carrier (2005) e Pollitt (2009), juntamente com as orientações estabelecidas pela ISO/IEC 27037:2012 e pelo NIST, abordam diferentes aspectos relacionados ao tratamento da evidência digital. Esses estudos contemplam desde a identificação das fontes de informação até os procedimentos necessários para sua preservação, análise e documentação.

A identificação, coleta, aquisição, preservação, análise e documentação constituem etapas relacionadas ao tratamento da evidência digital e devem ser conduzidas de forma organizada. A adoção de procedimentos adequados contribui para preservar as informações obtidas e possibilitar a verificação das ações realizadas durante a investigação.

Dessa forma, a utilização da evidência digital em investigações não depende apenas da localização de informações em dispositivos e sistemas. É necessário assegurar a preservação de sua integridade, registrar seu histórico e considerar seu contexto durante a análise, de modo que os dados obtidos possam contribuir de forma adequada para a compreensão dos fatos investigados.

---

# 3. Metodologia

A presente pesquisa caracteriza-se como aplicada, de abordagem qualitativa e caráter exploratório e descritivo, tendo como objetivo analisar as evidências digitais no contexto da computação forense. O estudo foi desenvolvido a partir da aplicação prática de procedimentos de identificação, coleta, aquisição, preservação e análise de dados provenientes de uma máquina virtual utilizada como ambiente controlado de investigação.

Inicialmente, foi realizada uma pesquisa bibliográfica para fundamentar os conceitos e procedimentos relacionados à evidência digital e à computação forense. Foram utilizadas obras acadêmicas e documentos técnicos, com destaque para Casey (2011), Carrier (2005) e Pollitt (2009), além das orientações do National Institute of Standards and Technology (NIST) e das normas ISO/IEC 27037:2012 e ISO/IEC 27042:2015.

Na etapa prática, foram identificadas as principais fontes de evidência disponíveis na máquina virtual, considerando arquivos, diretórios, registros do sistema, metadados, informações de usuários, aplicações e históricos de atividades. Posteriormente, os dados relevantes foram coletados e adquiridos de forma controlada, buscando minimizar alterações ou perdas das informações originais.

Para a preservação e verificação da integridade dos dados, foram utilizados mecanismos de controle, como funções de hash. Também foram registrados os procedimentos realizados durante a investigação, permitindo acompanhar o histórico da evidência desde sua identificação até as etapas de análise, de acordo com os princípios da cadeia de custódia.

Após a aquisição e preservação, os artefatos digitais foram analisados e correlacionados, considerando suas características, origem e relação temporal. Essa etapa teve como finalidade identificar informações relevantes e estabelecer possíveis relações entre arquivos, usuários, atividades e eventos, contribuindo para a reconstrução dos acontecimentos investigados.

Por fim, os resultados foram avaliados considerando a integridade das evidências, os valores de hash, os registros da cadeia de custódia e a documentação dos procedimentos realizados. Dessa forma, a metodologia permitiu relacionar os fundamentos teóricos da computação forense à aplicação prática em um ambiente computacional controlado, buscando assegurar a confiabilidade, a rastreabilidade e a preservação das evidências digitais analisadas.
