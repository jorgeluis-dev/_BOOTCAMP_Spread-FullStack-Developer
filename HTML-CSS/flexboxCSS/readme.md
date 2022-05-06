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

        }



}