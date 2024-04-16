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
    - 1.VeiculoTerrestre, 2.VeiculoAquático, 3.Carro, 4.Moto, 5.Barco, 6.NavioCargueiro, 7.Caminhão, 8.VeiculoAnfibio, 9.Submarino, 10.VeiculoAereo, 11.Aviao, 12.Veiculo, 13.HidroAviao, 
### Levantamento Requisitos





### Projeto OO e UML





### Diagrama de Caso de Uso





### Diagrama de Atividades




