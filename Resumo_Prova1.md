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

    - 




### Projeto OO e UML





### Diagrama de Caso de Uso





### Diagrama de Atividades




