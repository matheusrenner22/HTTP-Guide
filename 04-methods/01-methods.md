# HTTP Methods

* Define um conjunto de métodos HTTP
* Indica a ação que o cliente deseja operar
* Podem ser chamados de verbos HTTP
* Cada um possui a sua semântica
* Características
    * Seguro
        * Não altera o estado do servidor
        * Somente leitura
        * Cliente não solicita alterações
        * Não há carga extra para o servidor
        * O servidor é responsável em manter o método seguro
        * Quais são?
            * GET => GET / search.html HTTP/1.1
            * HEAD
            * OPTIONS
    * Idempotente
        * Ao executar o método, a resposta deverá ser sempre a mesma
        * Quais são?
            * Todos os seguros são idempotentes
            * PUT
            * DELETE
        * Status code poderá ser diferente
        * O servidor tem a responsabilidade de retornar dados da mesma maneira
        * Essa especificicação não é garantia de que todos os servidores irão aplicar o conceito corretamente


## Idempotence

HTTP method     IDEMPOTENCE     SAFETY

GET             yes             YES
HEAD            yes             YES
PUT             yes             
DELETE          yes
POST            NO
PATCH           NO