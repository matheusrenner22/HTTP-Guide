# PUT

* Criar um novo ou Atualiza um recurso
    * PUT /profile HTTP/1.1
    * Diferença entre POST?
    * Criação => status code 201
    * Atualização => status code 204 ou 200
* Características
    * Seguro: NÃO
    * Idempotente: Sim
    * BODY
        * Request: SIM
        * Response: NÃO
    * Uso em formulário HTML: NÃO
    * Cacheable: NÃO