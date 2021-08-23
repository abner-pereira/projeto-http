## HTTP (Hypertext Transfer Protocol)

### Markdown <br> https://www.markdownguide.org/basic-syntax/

### HTTP Tutoriais <br> https://developer.mozilla.org/en-US/docs/Web/HTTP

**Hypertext Transfer Protocol (HTTP)** é um protocolo de camada de aplicação para transmissão de documentos hipermídia, como o HTML. Foi desenvolvido para comunicação entre navegadores web e servidores web, porém pode ser utilizado para outros propósitos também. 

![imagem_web!](https://mdn.mozillademos.org/files/13677/Fetching_a_page.png  "Web em Geral")

### {JSON} Placeholder  <br> https://jsonplaceholder.typicode.com/
Free fake API for testing and prototyping.

**1. A typical HTTP session** <br>
Uma breve explicação de como funciona a conexão e comunicação utilizando o protocolo HTTP.

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Web/HTTP/Session

**2. URIs, URLs and URNs** <br>
A URI (Uniform Resource Identifier) é uma string que se refere a um recurso. Os mais comuns são URLs (Uniform Resource Locator), que identificam o recurso informando sua localização na web (Ex.: https://developer.mozilla.org). Os URNs (Uniform Resource Name), por outro lado, referem-se a um recurso por um nome, em um determinado namespace, como o ISBN de um livro (Ex.: urn:isbn:9780141036144).

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Web/HTTP/Resources_and_URIs
* https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Identifying_resources_on_the_Web
* https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_URL 

**3. HTTP Messages** <br>
São como os dados são trocados entre um servidor e um cliente. Existem dois tipos de mensagens:
requests (requisições) enviadas pelo cliente para acionar uma ação no servidor e responses (respostas), a resposta do servidor.

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages

**4. HTTP Headers** <br>
Permitem que o cliente e o servidor passem informações adicionais com a solicitação ou a resposta HTTP. Um HTTP header é composto por seu nome case-insensitive (não diferencia letras maiúsculas e minúsculas), seguido por dois pontos ':' e pelo seu valor (sem quebras de linha). Espaços em branco antes do valor serão ignorados.

Podem ser agrupados de acordo com seus contextos:
* Request headers - Contêm mais informações sobre o recurso a ser obtido ou sobre o cliente que está solicitando o recurso.
* Response headers - Contém informações adicionais sobre a resposta, como sua localização ou sobre o servidor que a está fornecendo.
* Representation headers - Contêm informações sobre o corpo do recurso, como seu tipo MIME ou codificação/compactação aplicada.
* Payload headers - Contêm informações independentes de representação sobre dados de carga útil, incluindo comprimento de conteúdo e a codificação usada para transporte.

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers

**5. HTTP Request Methods** <br>
O protocolo HTTP define um conjunto de métodos de requisição responsáveis por indicar a ação a ser executada para um dado recurso. Embora esses métodos possam ser descritos como substantivos, eles também são comumente referenciados como HTTP Verbs (Verbos HTTP). Cada um deles implementa uma semântica diferente, mas alguns recursos são compartilhados por um grupo deles, como por exemplo, qualquer método de requisição pode ser do tipo safe, idempotent ou cacheable (en-US).
* GET - O método GET solicita a representação de um recurso específico. Requisições utilizando o método GET devem retornar apenas dados.
* HEAD - O método HEAD solicita uma resposta de forma idêntica ao método GET, porém sem conter o corpo da resposta.
* POST - O método POST é utilizado para submeter uma entidade a um recurso específico, frequentemente causando uma mudança no estado do recurso ou efeitos colaterais no servidor.
* PUT - O método PUT substitui todas as atuais representações do recurso de destino pela carga de dados da requisição.
* DELETE - O método DELETE remove um recurso específico.
* CONNECT - O método CONNECT estabelece um túnel para o servidor identificado pelo recurso de destino.
* OPTIONS - O método OPTIONS é usado para descrever as opções de comunicação com o recurso de destino.
* TRACE - O método TRACE executa um teste de chamada loop-back junto com o caminho para o recurso de destino.
* PATCH - O método PATCH é utilizado para aplicar modificações parciais em um recurso.

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods

**5.1. Seguro** </br>
Um método HTTP é seguro se ele não altera o estado do servidor. Em outras palavras, um método é seguro se ele leva a uma operação de somente leitura. Diversos métodos de HTTP são seguros: GET, HEAD, ou OPTIONS. Todos os métodos seguros também são idempotentes, mas nem todos os métodos idempotentes são seguros. Por exemplo, PUT e DELETE são ambos idempotentes, entretanto são inseguros.

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Glossary/Safe/HTTP

**5.2. Idempotente** <br>
Um método HTTP é idempotente se uma requisição idêntica pode ser feita uma ou mais vezes em sequência com o mesmo efeito enquanto deixa o servidor no mesmo estado. Em outras palavras, um método idempotente não deveria possuir nenhum efeito colateral (exceto para manter estatísticas). Implementados corretamente, o GET, HEAD, PUT, e DELETE são métodos idempotentes, mas não o método POST. Todos os métodos  seguros também são idempotentes.

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Glossary/Idempotent

**5.3. Cacheable** <br>
Uma resposta armazenável em cache é uma resposta HTTP que pode ser armazenada em cache, que é armazenada para ser recuperada e usada posteriormente, salvando uma nova solicitação no servidor. Nem todas as respostas HTTP podem ser armazenadas em cache.

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Glossary/cacheable

**6. HTTP response status codes** <br>
Códigos de status retornados por uma requisição HTTP para o cliente. <br>
As respostas são agrupadas em cinco classes:
* Respostas informativas (100–199)
* Respostas bem-sucedidas (200–299)
* Redireciona (300-399)
* Erros do cliente (400–499)
* Erros de servidor (500–599)

Veja mais em:
* https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

Messages --- FALTA LER ESSE