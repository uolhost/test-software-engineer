# Teste De Conhecimentos para o perfil de Engenheiro de Software

Para que possamos conhecer um pouco mais sobre o seu trabalho, e mais especificamente sobre as suas habilidades de desenvolvimento de software, preparamos essa atividade simples, que poderá nos mostrar um pouquinho sobre a maneira que você organiza o seu código, a legibilidade dele, sobre seus conhecimentos básicos de MVC, ORM e banco de dados, se você utiliza bem Design Patterns, testes unitários, se faz TDD, etc.

# O problema:

Todos os dias, uma pessoa do time de desenvolvimento fica responsável pela resolução dos Incidentes.

*Exemplo*:

![Exemplo](/img/imday.png)

#### O que são os Incidentes?

São casos onde os clientes abrem chamado devido a determinados problemas, que podem ser sistemicos ou de entendimento de uso do produtos que cuidamos. Exemplo: Cliente contratou o produto de antivírus e não consegue utilizar o serviço. A pessoa responsável pela resolução do incidentes no dia, precisa analisar a situação da conta do cliente e verificar se existem falhas sistêmicas, e caso existam, gerar uma demanda para resolução definitiva.

# Necessidade:

- Expor uma API REST que possua os seguintes serviços:

    - No path	http://localhost:8080/im-day - Listar a ordem de resolução dos incidentes (conforme *exemplo*). A lista deverá conter o dia anterior, atual (hoje) e os próximos 9 dias. A lista das pessoas que resolvem os incidentes são: João, Maria, Zeca, Mario, Gustavo, Camila, Pedro, Juliana e Gisele. Supondo que dia 13/11 foi o dia do João, os dias subsequentes devem seguir a ordem a lista, sendo assim, Maria, dia 14/11, Zeca, 15/11 e assim por diante. Os dias não úteis (fds), não tem resolvedor. Sendo assim, necessário manter a ordem apenas nos dias úteis (segunda a sexta).

    - No path	http://localhost:8080/docs - Expor a documentação das APIs disponibilizadas.

- Expor um Painel (front-end) Angular que faça o consumo do serviço http://localhost:8080/im-day e exiba uma lista em formato tabela, no path http://localhost:4200. Criar um github a parte para este Painel.


# Requisitos Técnicos:

- Para a API Back-end:
    - Spring Boot (Java ou Kotlin);
    - Swagger e Swagger UI, para documentar os serviços;
    - JUnit ou outra ferramenta de testes de seu gosto/conhecimento;
    - Publicar o Projeto em sua conta no github;
    - Padronizar o Projeto/Arquitetura, de acordo com o seu conhecimento;
    - README do projeto, com instruções de uso.

- Para o Painel Front-end:
	- Angular e Bootstrap (Conhece React? Fique a vontade para utilizar);
	- Publicar o Projeto em sua conta no github (projeto diferente do acima);
	- Implementar testes de seu gosto/conhecimento (Selenium, por exemplo);
    - README do projeto, com instruções de uso.

# Desafios:

- Publicar a API no Heroku ou em qualquer outro serviço free disponível (conta free - https://devcenter.heroku.com/articles/deploying-spring-boot-apps-to-heroku)   
- Testes end-to-end dos serviços expostos, utilizando Cucumber ou outro framework de seu gosto/conhecimento;
- Persistir a lista de resolvedores Bancos de Dados relacional ou NoSQL de seu gosto/conhecimento;
- Criar o container (Docker) da Aplicação e Complementar o README com as instruções de uso.

# Observação: 

A descrição é breve propositalmente para que possamos avaliar sua criatividade. Não é obrigatório implementar todos os fluxos. Sinta-se a vontade para implementar, de acordo com o seu nível de conhecimento. Acreditamos que 7 dias (corridos), seja suficiente para implementar este teste. Nos envie a url dos projetos publicados no github. Se tiver alguma dúvida, nos procure (e-mail/skype/hangout).