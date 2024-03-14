# Funcionalidades de códigos prontos em JavaScript
## Gerar um relógio em tempo real
![código 1](img/primeiro%20código.png)

### Função startTime():
- Esta função é responsável por obter a hora atual, formatá-la e exibi-la na página web.
- Ela é chamada inicialmente usando ``document.write(startTime())`` dentro do elemento ``<div>``.

### Obtendo a hora atual:
- Cria um objeto ``Date`` chamado ``today`` que representa a data e hora atuais.

### Extraindo Componentes da Hora:
- Extrai as horas ``(h)``, minutos ``(m)`` e segundos ``(s)`` do objeto ``today``.

### Formatação da Hora (Opcional):
- O código inclui uma função opcional ``checkTime()`` (não chamada neste exemplo).
- Essa função adicionaria um zero à esquerda a qualquer componente de tempo menor que 10 (por exemplo, "9:00" em vez de "9:").

### Exibindo a Hora:
- Recupera o elemento com o ID "txt" usando ``document.getElementById()``.
- Define a propriedade ``innerHTML`` desse elemento para a string de hora formatada (concadeação de ``h``, ``m`` e ``s`` com dois pontos).

###  Definindo um Temporizador (Opcional):
- Esta linha está comentada no código fornecido.
- Se não for comentada, ela chamaria a função ``startTime()`` novamente após 500 milissegundos (meio segundo), efetivamente criando um loop que atualiza a hora exibida a cada meio segundo.

#### ``Resumindo, este código exibe a hora atual na página da web, com a opção de adicionar zeros à esquerda para melhorar a formatação. Se a linha do temporizador não for comentada, ela atualiza a hora dinamicamente a cada meio segundo.``


## Retirar os 5 últimos caracteres e adicionar uma nova palavra
![código 2](img/segundo%20código.png)

- Este código JavaScript altera uma string e a exibe na página da web.

### Declaração da String:
- Ambas as seções ``<script>`` contêm a linha ``var str = 'Terminal Root';``.
- Isso declara uma variável chamada ``str`` e a inicializa com a string "Terminal Root".

### Slicing da String:
- A linha ``str = str.slice(0, -5)+' Bash';`` é executada em cada ``<script>``.
- A função ``slice()`` é usada para extrair uma parte da string original ``str``.
- O primeiro argumento (``0``) indica o índice inicial (inclusive) da parte a ser extraída, que no caso é o início da string.
- O segundo argumento (``-5``) indica o índice final (exclusive) da parte a ser extraída. O valor negativo conta a partir do final da string, pegando tudo até cinco caracteres antes do final.
- O resultado é a string "Termina" (os primeiros cinco caracteres de "Terminal").
- O operador ``+`` concatena a string "Termina" com " Bash", resultando em "Terminal Bash".
- Importante notar que a variável str é reatribuída com o valor modificado a cada execução.

### Exibição da String:
- A linha ``document.write(str);`` é executada em cada ``<script>``.
- A função ``document.write()`` insere a string "Terminal Bash" no documento HTML, provavelmente no final da página da web (dependendo da localização do ``<script>``).

### Duplicação do Código:
- O código se repete em duas seções ``<script>`` separadas. Isso é redundante e alcança o mesmo resultado que ter em apenas uma seção ``<script>``.

### Resultado final:
- Devido à duplicação do código, o texto "Terminal Bash" seria exibido duas vezes na página da web.



