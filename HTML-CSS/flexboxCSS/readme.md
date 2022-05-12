#INTRODUÇÃO

Flexbox -> Modelo Layout unidimensional(oferece bom alinhamento dos itens)

flexCointaner{
    - Envolve os itens(possui filhos)
    - display: flex;
    - Conversão [Todo filho == Flex itens]

    PROPRIEDASS_FlexCointaner[
        - display = inicializador
        - flex-direaction = direcionamento
        - flex-wrap = aplica quebra de linha |OU| | NAO
        - flex-flow = direction_wrap
        - justify-content = alinha de acordo com a direção
        - align-items = alinha de acordo com o EIXO
        - align-content = alinha LINHAS CONTAINER
    ]
}

flexItem{
     - São os filhos diretos do Container
     - Pode se tornar FLEXCONTAINER (recursividade)
     - filhos com filhos | que podem ter filhos mais filhos que tem filhos

    PROPRIEDADES_FlexITEM{
        flex-grow = Define fator crescimento
        flax-basis = Define tamanho inicial |antes 
        flex-shrink = define a capacidade de redução
        flex = abreviação para 3 propriedades acima
        order = Ordem distribuição|listagem
        align-self = define alinhamento ITEM ESPECIFICO
    }
}
=======================================================================================
#FUNDAMENTOS FLEXBOX

1. Estrutura Basica {
        1#DISPLAYFLEX{

        }

        2#Flex-Direction{
            Define EIXO do ITEM
            linha(row) = [ESQUERDA => PARA DIREITA]
            row-reverse = [DIREITA => PARA ESQUERDA]

            coluna(column) = Ordenação de CIMA => PARA BAIXO
            column-reverse = DE BAIXO => PARA CIMA
        }

        Breakpoints{
            Dimensões, responsividade
        }


        3#Flex-WRAP{
            Define a quebra de linhas(container)

            nowrap [ padrão | não permite quebra de linha]

            wrap [Permite quebra-linha | ]

            wrap-reverse[permite quebra-linha | sentido contrario]

        }

}
=======================================================
flex-Flow => atalho para proriedades[flex-direction | flex-wrap]

========================

justify-content{
    Alinha itens[dentro container]

    flex-start [alinha inicio cointainer]
    flex-end [alinha final container]
    center: [ao centro]
    space-between [
        -> cria espaçamento igual entre elementos
    ]
    space-around[
        -> espaçamento do meio são duas vezes maior
    ]
}
================================================================
Align ITEMS

-> Alinhamento dos itens [EIXO CONTAINER]
-> Permite alinhar EIXO VERTICAL

types{
    center = alinha itens centro
    streth = padrão, flex itens crecem igualmente
    flex-start = alinha itens inicio
    flex-end = alinhamento dos itens no final
    baseline = alinha de acordo[ com a linha base tipografia dos itens]
}
===============================================
Align Content

-> Container utilize quebra de linhas
-> Altura do container > maior que a [SOMA] das linhas de itens

TYpes[
    center = itens ao centro
    stretch = padrão | flex itens crescem igualmente
    flex-start = itens no inicio
    flex-end = itens no final
    space-between = espaçamento igual entre os elementos
    space-around = espaçamento do meio | 2x | maior que o inicial_Final
]
===========================================
FLEX-SHRINK

Estabelece a capacidade de redução|
compressão do tamanho de um item
========================================================
FLEX{
    grow,shrik,basis;
    flex: 1, 0, auto
}

Align-Self{
    Alinha de modo individual sobre determinado item
}