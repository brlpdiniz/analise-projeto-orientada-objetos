## Resumo Prova 1 - APOO - Análise e Projeto Orientada a Objeto
### Profª: Marcia Regina M Cassitas Hino

| GRR | NOME |
| ------ | ------ |
| 2017208552 | Bruno Leandro Diniz |

### Introducao e Fundamentos OO
- O que é um sistema?
    - Sistema é um sistema é um conjunto de partes coordenadas para atingir um objetivo.
        - Sistema respiratório (respiração)

- Paradigmas
    - Um paradigma é um padrão, a forma como você soluciona um problemas.
    - Paradigma de programação é um meio de se classificar as linguagens de programação baseado em suas funcionalidades.
    - Entender os paradigmas auxilia o desenvolvedor a entender melhor e estruturar o sistema.
    - Exemplos:
        - Programação estruturada
        - Programação orientada a objeto

- Orientação a Objetos
    - Significa organizar o mundo real como uma coleção de objetos que incorporam estrutura de dados (atributos) e um conjunto de ações (métodos) que manipulam estes dados.
    - Conceitos:
        - Objetos: É uma entidade lógica que contém atributos e métodos
            - Atributos: são as características próprias dos objetos
                - Exemplo: nome da pessoa, cor do carro, valor da transação
            - Métodos: são blocos de instruções que manipulam os atributos
                - Exemplo: falar (pessoa), acelerar (carro), debitar (transação)

        - Classes: É uma estrutura de dados para declarar variáveis. Essa estrutura serve para definir objetos
            - Uma instância de uma classe é chamada de Objeto.
            - Definir uma classe não cria um objeto, assim como um tipo de variável não é uma variável.
    - Características:
        - Encapsulamento, Abstração, Herança e Polimorfismo

    > Classes não são Objetos, mas a estrutura de um Objeto


    Classe Cachorro {
        Atributos {
            raça:
            cor:
            altura:
        }
        Métodos {
            fazerCocô()
            crescer()
            latir()
        }
        return Objeto (conjunto de Atributo e Método)
    }

- EXERCÍCIO 1: Identifique as classes, atributos e métodos do cenário abaixo:
    João controla todo o gasto mensal da sua conta de luz em uma planilha eletrônica.
    Para cada conta de luz ele registra: data em que a leitura do relógio de luz foi realizada, número da leitura, quantidade de Kw gasto no mês, valor a pagar pela conta e data do pagamento.
    Mensalmente se pesquisam o mês de menor consumo e o de maior consumo

------------------------------------------------------------------------------------------------

- Encapsulamento
    - Um dado está encapsulado quando envolvido por código de forma que, só é visível na rotina onde foi criado.
    - Não interessa saber como é o funcionamento interno da classe e sim sua função. É como uma “caixa preta”.
    - Se refere ao agrupamento de dados com os métodos que operam nesses dados ou à restrição do acesso direto a alguns dos componentes de um objeto.
    - Exemplos:
        - Quando você aperta o botão “ligar” do aparelho remoto da televisão, você não sabe o que acontece, como o sinal chega na televisão, que circuitos são ativados, mas a televisão “liga”.
        - Quando você aperta o botão “play” do rádio, você sabe o que acontece? Como o som é emitido?
    
    - As opções de visibilidade que podem ser definidas em uma classe para atributos e serviços são:
        - (+) public: os elementos são acessíveis por todas as classes
        - (#) protected:os elementos são acessíveis por subclasses, ou pela própria classe
        - (-) private: os elementos são acessíveis somente pela própria classe

- Abstração
    - A abstração é o processo de filtragem de detalhes sem importância do objeto, para que apenas as características apropriadas que o descrevem permaneçam
    - Deve ser executada com algum objetivo para saber o que é importante e o que não é
    - Extrair tudo o que for essencial e nada mais
    - FLORESTA
        - Lenhador: tamanhoArea, quantidadeArvores, valorMercado / estimarValor(), venderLenha(), calcularLucro()
        - Passarinho: alimento, agua, ninho / comer(), beber(), dormir()

- Herança
    - Significa ser capaz incorporar os atributos e métodos de uma classe previamente definida.
    - Tem por objetivo criar uma hierarquia de objetos do mundo real, estabelecendo um relacionamento de pai e filho
    - Por meio da herança pode-se reutilizar ou alterar os métodos de classes existentes, bem como adicionar novos atributos a fim de adaptá-los a novas situações. Isso se chama especialização das classes
        - Herança simples: herda de um objeto
        - Herança múltipla: herda de vários objetos

- EXERCÍCIO 2: Organize hierarquicamente em um diagrama as seguintes classes:
    - 1.VeiculoTerrestre, 2.VeiculoAquático, 3.Carro, 4.Moto, 5.Barco, 6.NavioCargueiro, 7.Caminhão, 8.VeiculoAnfibio, 9.Submarino, 10.VeiculoAereo, 11.Aviao, 12.Veiculo, 13.HidroAviao

- EXERCÍCIO 3: Organize hierarquicamente em um diagrama as seguintes classes:
    - 1. MembroDaEscola, Professor, Coordenador, Funcionário, Ex aluno, CorpoDiscente (*), AlunoDaGraduacao, AlunoDaPosGraduacao, Atendente, CorpoDocente, Segurança
    - Discente é todo aluno regularmente matriculado, em regime de dependência ou trancado.

------------------------------------------------------------------------------------------------

- Polimorfismo
    - É o princípio pelo qual classes derivadas de uma mesma superclasse podem invocar o “mesmo” método, porém com comportamentos distintos para cada uma das classes derivadas.
    - Denota uma situação na qual um objeto pode se comportar de maneiras diferentes ao receber uma mensagem.
    - Consiste em utilizar o mesmo nome do método dentro de uma classe, ou em uma hierarquia de classes, com comportamentos diferentes.
    - É alcançado com auxílio do uso de herança nas classes e a reescrita de métodos das superclasses nas suas subclasses.

##### Fundamentos de Modelagem OO
- Descrição diagramática de algo a ser implementado em linguagem de programação
    - Modelagem prescritiva: antes do código
    - Modelagem descritiva: após o código

- Ato de criar uma representação de algo do mundo real por meio de modelos, simplificação da realidade:
    - Planta de uma casa representa mas não é a casa
    - Modelagem de sistemas: representações do sistema que estamos desenvolvendo

- OBJETIVOS:
    - Especificar estrutura e/ ou o comportamento do sistema.
        - Softwares complexos demandam planejamento. Os de baixa complexidade podem ser construídos direto.
        - Proporcionar guia para construção.
        - Documentar tomadas de decisões.

- VANTAGENS:
    - Descrição mais facilmente compreensível
        - Mais próxima da forma como as pessoas pensam
        - Não é natural “pensar” em linguagem de programação
    
    - Proporciona diferentes pontos de vista
        - Descrição dos elementos que compõem um programa (estrutura)
        - Descrição do programa em execução (dinâmica)
        - Possibilidade de visão global
        - Possibilidade de atenção a detalhes.

##### O QUE TEMOS QUE APRENDER PARA MODELAR EM OO?
- Conhecer os conceitos referentes a modelagem
    - Saber porque modelar
    - Conhecer os paradigmas de OO
    - Conhecer os requisitos de uma modelagem completa
    - Conhecer uma linguagem de modelagem
    - Ex: UML e todos seus diagramas

- Saber que passos seguir
    - Saber usar a linguagem de modelagem adotada

- Avaliar o que for produzido
    - Avaliar consistência do todo
    - Parâmetros de qualidade


### Levantamento Requisitos
- Primeiros passos para iniciar um sistema?
    - Levantamento de requisitos
    - É importante:
        - Identificar o problema a ser resolvido.
        -  Entender como o problema é tratado atualmente.
        -  Investigar soluções existentes no mercado (concorrentes).
        -  Perguntar aos usuários sobre a experiência atual.
        -  Identificar características de usabilidade.PÓ
    > Identifique necessidades dos usuários e estabeleça requisitos.

- Requisitos
    - É um mapeamento do que se espera que o sistema apresente.
    - É uma condição ou capacidade para a qual um sistema deve atender.
    - É como se fosse uma espécie de declaração de o que o sistema deve ter ou de como deveria operar.
    - Não é fácil:
        - Entender as funcionalidades;
        - Listar necessidades futuras;
        - Entender problemas que você não está familiarizado;
        - Entender detalhes de processos;
        - Ter a visão do todo.

    - Exemplos de requisitos:
        - Funcionalidades ao nível do usuário
            - Emitir certificado de participação do aluno no evento da semana pedagógica.
        - Propriedades gerais do sistema
            - O sistema deverá manter um registro de toda consulta e alteração no cadastro.
        - Uma regra de negócio
            - A nota do aluno será a média aritmética simples entre as notas parciais.
        - Restrições do sistema ou do seu desenvolvimento
            - O sistema deve ser desenvolvido com ferramentas Microsoft®.
            - O sistema deve atender as normas de acessibilidade existentes.
    Atenção!
        - O levantamento pode indicar visões diferentes e necessidades contraditórias;
        - Usuários geralmente conhecem muito do negócio e pouco de sistema, enquanto que os analistas conhecem muito de sistemas e pouco do negócio;
        - Usuários podem omitir informações, acreditando que é algo óbvio. 

    - Requisitos são importantes para projetos de TI, pois são a base para:
        - Definição de contratos;
        - Elaboração/análise de propostas;
        - Planejamento de atividades;
        - Estimativas de custo;
        - Modelagem do sistema;
        - Desenvolvimento das funcionalidades.

    - Sendo assim....
        - O mapeamento e entendimento completo dos requisitos é fundamental para se obter um sistema e um processo de desenvolvimento de qualidade.
        - O sistema deve ser desenvolvido de maneira a evoluir para atender necessidades futuras eminentes dos usuários, mesmo que não seja um requisito claro por parte deles.
        - O objetivo do requisito é que seja completo o suficiente para que o desenvolvimento possa ser realizado e que se possa validar com o usuário se o que está sendo entregue é o que foi solicitado, e se atende sua necessidade.
    
    1. Requisitos Funcionais (RF)
        - Funcionalidade (funções que o sistema deve realizar)
        - Serviços (que se espera que o sistema faça)
    2. Requisitos Não Funcionais(RNF)
        - Qualidade
        - Tipos:
            * Requisitos do Produto:
                - Especificam o comportamento do software (ex.: eficiência, desempenho, segurança, portabilidade, usabilidade, confiabilidade).
                - “A base de dados deve ter acesso apenas de usuários autorizados”.
            * Requisitos Organizacionais:
                - Consequência de políticas e procedimentos das empresas (ex.: padrões do cliente)
                - O processo de desenvolvimento deve estar de acordo com normas ISO 9126”.
                - O prazo de entrega final do sistema é de 3 meses”.
            * Requisitos Externos:
                - Derivados do ambiente ou fatores externos ao sistema (ex.: legislação)
                - O sistema deverá se comunicar com o SQL Server” (interoperabilidade).
                - O sistema deverá atender às normas legais, tais como padrões, leis, etc” (legal).
                - O sistema não apresentará aos usuários quaisquer dados de cunho privativo” (ético).
    
    - Requisitos Técnicos
        - Recursos necessários para que a aplicação possa operar, tais como processamento, memória, armazenamento, link de comunicação.
        * COMPATIBILIDADE: aplicação deve rodar independente da arquitetura e do dispositivo que a esteja hospedando.
        * DISPONIBILIDADE: Que tipo de informação é necessário acesso em tempo real?
            - Que tipo de informação pode haver um atraso? Qual o tamanho deste atraso?
        * ARMAZENAMENTO: •Por quanto tempo registros antigos devem ser mantidos?
    
    - Requisitos Ambientais
        - AMBIENTE SOCIAL: Fisicamente próximas? Existe necessidade de colaboração de dados?
            - Síncrono ou assíncrono? Como será a comunicação?
        - AMBIENTE ORGANIZACIONAL: Hierarquia, Estrutura técnica (funcionários e equipamentos)
            - Implantação de projetos, Investimentos em tecnologia?
        - AMBIENTE TÉCNICO: Quais são as tecnologias utilizadas? O que precisa manter a compatibilidade?
            - Limitações tecnológicas?

    - Atividade: Identifique os requisitos funcionais e não funcionais:
        - “Um aplicativo de celular de emissão de passagens vende passagens de trem e avião. Quando o usuário entra no aplicativo, um menu com os possíveis destinos é mostrado ao usuário, junto com uma mensagem para que o usuário selecione um destino. Os usuários podem escolher seu destino a partir dessa lista. Os destinos sugeridos devem ser organizados de maneira a facilitar a escolha pelo usuário. Após a escolha do destino, o sistema deve responder prontamente se há poltrona disponível. Somente após essa verificação é solicitado ao usuário que informe o número de seu cartão de crédito e o código de segurança. O cartão é validado. Quando a transação de crédito é validada, a passagem é emitida. O formato do bilhete de passagem deve seguir o padrão definido pelo Sistema Nacional de Tráfego Ferroviário ou pelo Sistema Nacional de Tráfego Aéreo, a depender do transporte escolhido”.

------------------------------------------------------------------------------------------------

- Técnicas de levantamento de requisitos
    - Objetivo:
        - Ajudar os analistas de sistemas e negócio na condução do levantamento de requisitos do sistema.
    - Atividades envolvidas:
        - Identificar os objetivos
        - Selecionar o público alvo adequado
    - Qual técnica usar? Analisar:
        - Recursos disponíveis($$$)
        - Tempo disponível(para execução e compilação de resultados)
        - Disponibilidade de usuários(presencial, remota etc)
    - Técnicas de levantamentov:
        - Entrevistas
            * Obter informações que não são registradas e estão concentradas em algumas pessoas.
            * Obter a opinião das pessoas sobre o sistema.
            - Recomendações
                - Não atrase.
                - Explique o objetivo da pesquisa para conquistar a confiança do entrevistado.
                - Escute mais que pergunte.
                - Vá preparado. Evite ler as perguntas do roteiro.
                - Tomar notas durante a entrevista.
                - Fazer o relatório da visita e validar as informações.
        - Questionário
            * É um formulário que pode ser distribuído impresso ou on-line com perguntas que os usuários e demais participantes.
            * Otimizar o entendimento do processo se um grande número de pessoas deve ser entrevistado e não há recursos para entrevistá-las individualmente.
            * Quando há diversos grupos de usuários que podem estar em localizações geográficas diferentes.
            > Inclua sempre uma alternativa “sem opinião”.
            > Não sei responder.
        - Observação
            * O observador é inserido no ambiente de trabalho onde a solução será usada observando o trabalho cotidiano e tomando notas das tarefas em execução nas quais as partes interessadas estão envolvidas.
            * Quando usar?
                - Para avaliar o processo de trabalho existente.
                - Para melhorar ou modificar o sistema atua.
                - Descobrir problemas de performance.
                - Confirmar dados recolhidos na entrevista.
            * Recomendações:
                - Deve ocorrer preferencialmente em um período em que o serviço seja caracterizado como normal, para não haver distorções;
                - O observador deve colocar-se no ambiente sem interferir,
                - O observador não deve fiscalizar o trabalho;
        - Reunião
            * Comunicação direta entre as partes interessadas
            * Integração do grupo em torno do mesmo assunto, formando uma equipe de trabalho
            * Coleta de sugestões e críticas da equipe
            * Quando usar?
                - obter uma resposta rápida de várias pessoas sobre um determinado assunto;
                - para resolução de problemas ou questões a serem esclarecidas, compartilhadas com os demais participantes;
                - para envolver o grupo da tomada de decisão;
                - para resolver situações de conflito (busca de consenso);
            * Recomendação:
                - Não defender suas ideias ao extremo; não mostrar contrariedade; não mudar de opinião para evitar conflitos
        - Brainstorming
            * “tempestade de ideias”
            * Gerar ideias e selecionar
            * Explicar as regras:
                - Não critique!
                - Não avalie!
                - Seja aberto a todas as ideias, mesmo aquelas que parecerem malucas.
                - Escrever as ideias dos participantes no quadro.
        - Cenários
        - Protótipos

    - QUAIS OS PROBLEMAS NO LEVANTAMENTO DE REQUISITOS?
        - NÃO VER O TODO: REQUISITOS AUSENTES OU SUBENTENDIDOS.
        - FALTA DE COMPLETUDE OU INCONSISTÊNCIA.
        - FALTA DE CLAREZA, PERMITINDO INTERPRETAÇÕES DÚBIAS.
        - FALTA DE DEFINIÇÃO CLARA DE RESPONSABILIDADES.
        - FALTA DE ENVOLVIMENTO DO USUÁRIO.
        - DIFICULDADE PARA ENTENDER O PROBLEMA.
        - MUDANÇA DE OBJETIVOS.
        - FUNCIONALIDADES ADICIONAIS AOS REQUISITOS. (XÍCARA DE OURO)

    - Em relação às fontes de informação
        - Stakeholders
            * Disponibilidade / Restrições de contato
        - Sistema atual
            * Disponibilidade para consulta / Documentação / Manual.
        - Perspectivas de futuro
        - Leis / Regulamentações
        - Normas
            * O que deve ser seguido
        - Regras da organização

### Projeto OO e UML





### Diagrama de Caso de Uso





### Diagrama de Atividades




