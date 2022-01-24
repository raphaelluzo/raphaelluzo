# 📕 Características e Benefícios

![](<.gitbook/assets/image (1).png>)

## Características:&#x20;

1. A lógica da aplicação é quebrada em pequenos componentes que possuem limites de atuação muito bem definidos e que trabalham de forma coordenada para entregar uma solução
2. Dentro dessa solução, cada componente possui um pequeno domínio de responsabilidade e sua implantação é independente de qualquer outro componente.
3. Cada micro serviço possui responsabilidade por uma pequena parte do domínio de negócio e devem ser reutilizáveis em múltiplas plataformas.
4. Micro serviços se comunicam seguindo alguns princípios básicos e utilizam protocolos de comunicação considerados leves, como o HTTP. Para a troca de dados, o JSON se tornou um padrão.
5. A tecnologia utilizada no desenvolvimento é irrelevante porque as aplicações que irão se comunicar com o micro serviço sempre irão se comunicar com uma linguagem que possui um protocolo neutro.
6. Com isso, micro serviços podem muito bem ser desenvolvidos com múltiplas linguagens e tecnologias.
7. Como os micro serviços, por natureza, são pequenos, independentes e distribuídos as organizações podem formar pequenos times com responsabilidades bem definidas dentro de áreas específicas de negócio.
8. Esses times trabalharão com a meta de entregar uma aplicação completa, porém, cada um atuará apenas no campo em que seu time é responsável.

## Benefícios:&#x20;

**Alta Coesão:** Um dos princípios da arquitetura de microsserviços é a alta coesão, o serviço deve ter um único foco. Ou seja, ter uma única responsabilidade do domínio da aplicação. Este princípio é útil para controlar o tamanho e impedir que o microsserviço se torne um serviço monolítico.

**Resiliência:** Não importa a velocidade e os custos das soluções, é importante construir sistemas que reajam a falhas inesperadas. Ser capaz de validar os dados recebidos (mesmo que estes estejam corrompidos) e tratar a perda ou falha na comunicação com outro serviço da cadeia, sem quebrar o fluxo da aplicação.

**Observável:** Poder acompanhar o status do sistema e conseguir observar o que está acontecendo em tempo real. Esse tipo de monitoramento precisa ser centralizado para facilitar a busca de informações sobre o status atual do sistema. Como microsserviços é uma arquitetura distribuída, a ideia de centralizar o monitoramento, principalmente os logs, facilita verificação do ciclo completo de toda mensageria trocada. Desde a primeira iteração do usuário até a solução entregue pela aplicação.

**Automatização:** Com a divisão de uma aplicação entre diversos mini blocos há uma necessidade maior de automatizar algumas tarefas para manter este tipo de arquitetura. Como integração contínua e entrega contínua. Esse é um dos aspectos que fazem esse modelo ser abraçado por defensores da cultura DevOps. Pois esta é a ideia principal que move essa cultura.

**Centrado no domínio do negócio:** Um microserviço deve estar focado no domínio do negócio. Assim sendo, deve ser uma função do negócio. Quem conhece o padrão de desenvolvimento DDD sabe que o domínio é o coração de uma aplicação. O conceito base que alicerça este pensamento é o que no DDD chamamos de Bounded Context (ou contextos delimitados). Os contextos delimitados servem para refatorar um grande domínio em pequenos conjuntos de domínios que unidos representam o modelo de negócio de uma aplicação. E é exatamente essa característica um dos pontos fundamentais no modelo de microsserviços.

**Escala Independente:** Cada microsserviço pode escalar independentemente via eixo X escalonamento (clonagem com mais CPU ou memória) e eixo Z dimensionamento (fragmentação), com base no que é necessário. Isto é muito diferente das aplicações monolíticas, que podem ter requisitos muito diversos, mas ainda devem ser implantados juntos como uma única unidade.

**Atualização Independentes:** Cada serviço pode ser implantado independentemente de outros serviços. Qualquer alteração local em um serviço pode ser feita facilmente por um desenvolvedor sem exigir coordenação com outras equipes. Por exemplo, para atender negócios em constante mudança requisitos, um serviço pode ser melhorado substituindo o implementação anterior. Como resultado, isso melhora a agilidade do microserviço. Este também é um ótimo facilitador de Integração Continua / Entrega Continua.

**Manutenção Fácil:** O código em um microsserviço é restrito a um recurso e com isso mais fácil de entender. IDEs podem carregar menores quantidades de código e com menos código, aumenta a facilidade do desenvolvedor da manutenção.

**Tecnologia poliglota:** Os desenvolvedores são livres para escolher a linguagem e a pilha tecnologica mais adequada para construção do serviço. Eles são livres para inovar dentro do limites de seu serviço. Isso permite reescrever o serviço usando novas tecnologias, em vez de ter que manter decisões passadas, dando assim a liberdade de escolha de tecnologias, ferramentas ou estruturas.

**Isolamento de falhas e recursos:** Um serviço mal comportado, como um “memory leak” ou uma falta de gerenciamento do pool de conexões de banco de dados, pode afetar o serviço por completo, caso a aplicação tiver arquitetura monolítica. Com microsserviços bem projetados, as falhas podem ser isoladas em um único serviço e não se propagam para o resto do sistema, permitindo um isolamento de falhas que comprometem a aplicação por completo.

**Melhor comunicação entre equipes:** Um microsserviço é normalmente construído por uma equipe que domina a pilha tecnológica por completo. Todos membros relacionados a um domínio trabalham juntos em uma única equipe,o que melhora significativamente a comunicação entre os membros da equipe, como eles compartilham os mesmos objetivos finais, entregam o serviço no ambiente de produção.

**Monitoramento de serviços:** Um dos aspectos mais importantes de um sistema distribuído é o monitoramento e registro de serviços. Isso permite que você tome ação proativa se, por exemplo, um serviço estiver consumindo recursos inesperados. Agregar logs de diferentes microsserviços e fornecer uma visualização consistente. Fazer com que os dados disponíveis para usuários corporativos.

**Devops:** Integração Contínua e Implantação Contínua (IC / EC) são muito importantes para que os microsserviços possam ter sucesso. Essas práticas são necessárias para que os erros possam ser identificados, cedo por meio de testes automatizados e pipelines de implantação.

**Pequenas equipes direcionadas** : as equipes podem ser direcionadas para apenas um serviço, tornando o código mais fácil de entender e facilitando a entrada de novos membros na equipe, sem a necessidade de passar semanas descobrindo como funciona um monólito complexo. Também promove a flexibilidade, equipes grandes tendem a ser menos produtivas porque a comunicação é mais lenta, o tempo de gerenciamento aumenta e a agilidade diminui.

**Base de código pequena** : em um aplicativo monolítico, as dependências de código tendem a se misturar com o tempo. A adição de novas funcionalidades requer a alteração do código em muitos lugares. Em uma arquitetura de microsserviços, que não compartilha código ou banco de dados, essas dependências são minimizadas, o que facilita a adição de novos recursos. Também complementa o ponto anterior que facilita o entendimento do código e a introdução de novos membros na equipe.

**Isolamento de dados** : Em uma arquitetura de microsserviços, cada serviço tem acesso privado ao seu banco de dados (idealmente), podemos então realizar uma atualização do esquema do banco de dados sem afetar os outros serviços. Em um aplicativo monolítico, as atualizações de esquema podem se tornar muito difíceis e arriscadas, pois várias partes do aplicativo podem usar os mesmos dados.

**Avanços tecnológicos** : avanços recentes em tecnologias de nuvem e conteinerização tornam a configuração de uma arquitetura de microsserviços cada vez mais simples. Todo provedor de nuvem tem soluções para esse tipo de arquitetura para facilitar a vida dos desenvolvedores.

**Lançamento no mercado com mais rapidez**: Como os ciclos de desenvolvimento são reduzidos, a arquitetura de microsserviços é compatível com implantações e atualizações mais ágeis.

**Altamente escalável**: À medida que a demanda por determinados serviços aumenta, você pode fazer implantações em vários servidores e infraestruturas para atender às suas necessidades.

**Fácil de implantar**: Como as aplicações baseadas em microsserviços são mais modulares e menores do que as aplicações monolíticas tradicionais, as preocupações resultantes dessas implantações são invalidadas. Isso requer uma coordenação maior, que pode ser alcançada com uma camada de service mesh, mas as recompensas podem ser extraordinárias.

**Acessível**: Como a aplicação maior é decomposta em partes menores, os desenvolvedores têm mais facilidade para entender, atualizar e aprimorar essas partes. Isso resulta em ciclos de desenvolvimento mais rápidos, principalmente quando também são empregadas as metodologias de desenvolvimento ágil.

**Mais open source**: Devido ao uso de APIs poliglotas, os desenvolvedores têm liberdade para escolher a melhor linguagem e tecnologia para a função necessária.

{% hint style="info" %}
Agora que temos uma ideia melhor de todas as vantagens de uma arquitetura de microsserviços, vamos ver quais são as desvantagens e os desafios:

**Complexidade** : Enquanto cada serviço é mais simples, o sistema como um todo é mais complexo. Como este é um sistema distribuído, deve-se tomar cuidado para selecionar e configurar todos os serviços e bancos de dados e, em seguida, implantar cada um desses componentes de forma independente. Todos os desafios de um sistema distribuído devem ser levados em consideração.

**Teste** : Ter vários serviços independentes pode tornar a escrita de testes mais complexa, especialmente quando há muitas dependências entre os serviços. Uma simulação deve ser usada para cada serviço dependente para poder testar um serviço de unidade.

**Integridade dos dados** : os microsserviços têm uma arquitetura de banco de dados distribuída, o que é um desafio para a integridade dos dados. Algumas transações comerciais, que exigem a atualização de várias funções comerciais do aplicativo, precisam atualizar vários bancos de dados pertencentes a diferentes serviços. Isso requer a configuração de consistência eventual de dados, o que obviamente é mais complexo e menos intuitivo para os desenvolvedores.

**Latência de rede** : o uso de muitos serviços pequenos pode resultar em maior comunicação entre os serviços. Além disso, se você tiver uma cadeia de dependência entre serviços para realizar uma transação comercial, a latência adicional resultante pode se tornar um problema. As comunicações assíncronas devem ser favorecidas quando o uso permitir, mas isso mais uma vez adiciona complexidade ao sistema.

De acordo com estas vantagens e desvantagens é então mais ou menos relevante adotar uma arquitetura de microsserviços, não existe uma regra universal, cada projeto é único e as motivações para uma ou outra arquitetura dependem das necessidades e do contexto da mesma.
{% endhint %}



####
