# Refatora-o
Código refatorado baseada nas aulas ministradas pelo professor malvezzi

# Estrutura de Código
A estrutura do projeto foi reorganizada para melhorar a legibilidade e modularidade do código. Cada função tem uma responsabilidade única, facilitando a manutenção e testes individuais de cada módulo.

-> main(): Função principal do programa, responsável pela inicialização e controle do fluxo do jogo.
-> mostrarForca(): Exibe o estado atual da forca com base nos erros do usuário.
-> validarTentativa(): Realiza a leitura e validação segura da tentativa do usuário.
-> verificarPalavraCompleta(): Verifica se a palavra secreta foi totalmente adivinhada.
-> Funções auxiliares para manipulação de strings e controle do jogo.
## Boas Práticas e Melhorias Implementadas
# Código Duplicado
-> Problema: O código original apresentava duplicação significativa nas estruturas de exibição da forca e nas mensagens de erro.
->Solução: Foi criada a função mostrarForca para centralizar a exibição da forca e uma lista de strings para centralizar mensagens, eliminando cerca de 20 linhas de código duplicado.
# Segurança
-> Uso de gets(): A função gets() foi substituída por fgets() para evitar vulnerabilidades de buffer overflow, aumentando a segurança da entrada de dados.
-> Limpeza de Buffer com fflush(stdin): A prática de usar fflush(stdin) foi removida, pois não é garantida em todas as plataformas. Em vez disso, foi implementado um método portátil para limpeza do buffer de entrada.
# Modularização
-> Problema: O código original estava diretamente na função main, sem modularização adequada.
-> Solução: O código foi dividido em funções menores, cada uma com uma responsabilidade única, melhorando a organização e facilitando a manutenção e reutilização.
# Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue para reportar bugs ou sugerir melhorias, ou submeter um pull request.
