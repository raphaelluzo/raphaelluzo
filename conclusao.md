# 📙 Conclusão

Guarde essas informações. Elas são muito, muito **importantes**.

Quando uma organização está considerando a possibilidade de construir uma aplicação com arquitetura orientada a micro serviços é necessário ficar de olho nos pontos abaixo:

**Primeiro ponto,** micro serviços são sistemas distribuídos e auto contidos (eu sei que tá chato ficar repetindo isso, mas é necessário), isso traz um certo grau de complexidade para sua aplicação que não existiria em sistemas monolíticos.

Uma arquitetura orientada a micro serviços requer um alto grau de maturidade operacional.

Então, se sua organização não está disposta a investir em automação de processos e trabalhos operacionais, como monitoramento e escalonamento de recursos, não seria uma boa ideia considerar esse tipo de arquitetura. Sacou?

O **segundo ponto** chave a ser levado em consideração é a grande expansão de servidores ou containers necessários para a implantação dos micro serviços.

O modelo mais comumente utilizado é um container para cada micro serviço, então você pode imaginar que, com o tempo e crescimento da aplicação, um sistema com esse modelo de arquitetura poderá ter entre 50 e 100 servidores que precisarão ser mantidos e monitorados em ambiente de produção.

Isso traz uma complexidade operacional enorme e precisará ser colocada na balança no momento de decidir usar ou não uma arquitetura orientada a micro serviços.

O **tipo de aplicação** é outro fator importantíssimo a ser levado em conta, pois esse modelo é para grandes aplicações.

Por isso, se sua aplicação é pequena, departamental ou possui um pequeno número de usuários, utilizar uma arquitetura orientada a micro serviços pode não valer a pena.

![](<.gitbook/assets/image (3).png>)
