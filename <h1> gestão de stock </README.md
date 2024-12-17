<h1> gestão de stock </h1>
A função adicionar_material tem o objetivo de adicionar um material a um estoque (representado pela variável stock, que provavelmente é um dicionário onde as chaves são os nomes dos materiais e os valores são as quantidades disponíveis). A função faz o seguinte:

Recebe o nome do material: O utilizador é solicitado a inserir o nome do material.
Verifica se o material já existe no estoque: Se o material já estiver no estoque (isto é, se o nome já for uma chave no dicionário), o programa avisa o utilizador de que o material já existe e não faz nada.
Adiciona um novo material: Se o material não existir no estoque, o programa pede a quantidade inicial do material, e depois adiciona essa informação ao estoque.
Valida a quantidade: Caso o utilizador insira um valor inválido para a quantidade (como texto ou um número negativo), o programa emite uma mensagem de erro.

A função consultar_stock que você forneceu está bastante clara e bem estruturada. Ela serve para consultar a quantidade de um material específico no estoque (representado pelo dicionário stock). Vou explicar o que ela faz e, em seguida, traduzi-la para o português de Portugal, caso necessário.

O que a função faz:
Recebe o nome do material: O utilizador insere o nome do material que deseja consultar no stock.
Verifica se o material existe no stock: A função verifica se o nome inserido está presente no dicionário stock.
Exibe o stock: Caso o material esteja no stock, a função mostra a quantidade atual desse material.
Mensagem de erro: Se o material não estiver no stock, a função avisa o utilizador de que o material não foi encontrado.

A função atualizar_stock que você forneceu serve para adicionar ou remover unidades de um material já existente no estoque, dependendo da escolha do utilizador. Vamos detalhar o que a função faz e depois adaptá-la para o português de Portugal, se necessário.

O que a função faz:
Recebe o nome do material: O utilizador insere o nome do material a ser atualizado no estoque.
Verifica se o material existe no estoque: Se o nome do material for encontrado no dicionário stock, o código segue para o próximo passo. Caso contrário, exibe uma mensagem informando que o material não foi encontrado.
Escolha da operação: O utilizador escolhe se deseja adicionar unidades ao estoque (A para adicionar) ou remover unidades do estoque (R para remover).
Adiciona ou remove unidades:
Se a operação for adicionar (A), a quantidade inserida é somada ao estoque do material.
Se a operação for remover (R), a função verifica se há unidades suficientes no estoque. Se houver, as unidades são removidas. Caso contrário, o sistema informa que a quantidade disponível é insuficiente.
Mensagem de erro: Se a operação escolhida não for válida (nem "A" nem "R"), o código informa que a operação é inválida.

A função exibir_stock que você forneceu tem como objetivo exibir o estado atual do estoque (representado pelo dicionário stock), mostrando todos os materiais e suas respectivas quantidades. Vou explicar o que ela faz e, em seguida, ajustá-la para o português de Portugal, se necessário.

O que a função faz:
Imprime um cabeçalho informativo: O texto "Estado Geral do Stock" é exibido, seguido de uma tabela que mostra as colunas "Material" e "Quantidade".
Exibe os materiais e as quantidades: A função percorre o dicionário stock e exibe cada material e a sua quantidade associada. Cada linha é formatada com o nome do material seguido pela quantidade.
Formatação de exibição: Utiliza o caractere de tabulação (\t) para formatar as colunas de maneira alinhada, tornando a visualização mais organizada.

O código que você forneceu para a função main implementa um menu interativo para o gerenciamento de um estoque. A função oferece opções para adicionar, consultar, atualizar, e exibir o estoque, e também tem a possibilidade de encerrar o programa.

O que a função faz:
Menu interativo: O código exibe um menu com as seguintes opções:

Adicionar material ao estoque.
Consultar o estoque de um material específico.
Atualizar o estoque de um material (adicionar ou remover unidades).
Exibir o estoque geral (todos os materiais e suas quantidades).
Sair do programa.
Processamento de entrada: O utilizador escolhe uma opção inserindo um número correspondente. Dependendo da escolha, a função chama a função apropriada (adicionar_material, consultar_stock, atualizar_stock, exibir_stock) para realizar a ação solicitada.

Loop infinito: O menu continua sendo exibido em um loop (while True) até que o utilizador escolha a opção "5" para sair, que faz o programa terminar.
