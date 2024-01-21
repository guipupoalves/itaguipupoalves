# Projeto de conclusão de curso - ITA - Desenvolvimento Ágil de Software

Arquivo completo (diagramação, gráficos e imagens) disponível em PDF.

1.  Introdução


Esse é um portal onde os usuários podem marcar livros que já tenham lido. Fazendo isso, ganham pontos dentro de um sistema de gameficação com ranking de leitura.
Cada livro lido gera 1 (um) ponto, sendo que a cada 100 páginas que o livro tiver ele vale um ponto adicional (Exemplos: 72 páginas valem 1 ponto, 124 páginas valem 2 pontos, 350 páginas valem 4 pontos).
A cada 5 livros que o usuário ler de um mesmo estilo, ele receberá um troféu exclusivo daquela categoria!! Por exemplo: se ele leu 5 livros do estilo "Ficção Científica", ganhará o troféu "Leitor de Ficção Científica".

2.  Estruturação de User Stories e Testes de aceitação

Neste presente trabalho, a escala adotada para o cálculo de Business Value é representada por x∈R | 1 ≤ x ≤ 10. Desse modo, o menor valor possível para o valor de negócio de uma User Story será representado por 1, e o maior valor possível será representado por 10.

a.  Logar Usuário: Eu, como usuário da aplicação, quero poder realizar login na mesma para que eu possa acessar as funcionalidades e recursos disponibilizados.

Size: Pequeno
Business Value: 3 
Teste de aceitação: O login deve ser realizado através da coleta de informações de usuário e senha válidos, de modo que, caso quaisquer dos parâmetros esteja incorreto, não seja possível prosseguir o processo de autenticação e acessar a aplicação.

b.  Visualizar lista de livros: Eu, como usuário da aplicação, quero poder visualizar a lista completa de livros, para que eu possa saber quais estão disponíveis na aplicação.

Size: Mediano
Business Value: 7
Teste de aceitação: A visualização da lista deve permitir acesso individual a qualquer um dos livros nela contida para obter mais informações sobre o mesmo. Deve ser possível rolar a lista utilizando o scroll up/down do mouse. 

c.  Visualizar livro: Eu, como usuário da aplicação, quero poder visualizar um livro específico da lista, para que eu possa saber mais informações sobre o mesmo, como sinopse, número de páginas e gênero da obra.

Size: Mediano
Business Value: 7
Teste de aceitação: Durante o acesso a lista de livros, deve ser possível clicar individualmente em um livro para acessar mais informações sobre o mesmo, como: Sinópse, número de páginas e gênero.

d.  Marcar leitura de livro: Eu, como usuário da aplicação, quero poder marcar um livro específico da lista que eu já tenha lido, para que eu possa ganhar os pontos provenientes da leitura.

Size: Mediano
Business Value: 9
Teste de aceitação: Na página de um livro específico, deve ser possível marcar o mesmo como lido ao clicar no botão “Esse eu já li!”, bem como sua pontuação deve ser devidamente contabilizada no perfil do usuário para sua consideração pessoal e no ranking.

e.  Visualizar ranking de usuários: Eu, como usuário da aplicação, quero poder visualizar o ranking de usuários, para que eu possa comparar minha pontuação com os demais leitores.

Size: Mediano
Business Value: 6
Teste de aceitação: Deve ser possível através da home acessar uma página de rank que classifica os usuários em ordem decrescente de pontuação. O rank deve ser constituído por até 10 usuários, onde os 3 primeiros terão um destaque maior.

f.  Visualizar pontos e troféus de usuário: Eu, como usuário da aplicação, quero poder acessar o meu perfil e visualizar meus pontos e troféus coletados ao longo do uso da aplicação, para que eu possa ter um controle efetivo no meu progresso.

Size: Mediano
Business Value: 6
Teste de aceitação: Durante ao acesso de login do usuário, deve ser possível visualizar sua pontuação de leitura, bem como quais troféus foram adquiridos pelo mesmo.


3.  Modelagem e Diagramação

A modelagem e diagramação foi realizada para facilitar o entendimento da aplicação, bem como auxiliar na compreensão do funcionamento do sistema.

3.1 –Explicação do fluxo das User Stories

User Story: Fazer login


Usuário insere seu nome no campo “Usuário” e sua senha no campo “Senha”, logo após clicar em “Entrar”. Caso ambos parâmetros estejam corretos, o processo de autenticação é realizado com sucesso e o usuário é redirecionado para a página da home.


User Story: Visualizar lista de livros

Ao clicar na opção destacada “Lista de livros disponíveis” o usuário será redirecionado para a lista contendo todos os livros disponíveis na aplicação:


User Story: Visualizar Livro

Na página de lista dos livros, o usuário pode selecionar um livro específico para receber mais informações sobre o mesmo ao clicar no botão com o título e autor logo abaixo da ilustração de sua capa.

Ao realizar tal operação, o usuário será redirecionado para a página do livro desejado, que contém informações sobre o mesmo:



User Story: Marcar leitura de livro
 
Na página específica do livro o usuário pode clicar no botão em destaque “Esse eu já li” para confirmar sua leitura e contabilizar os pontos referentes ao livro em seu perfil.



User Story: Visualizar ranking de usuários

Na página inicial, ao clicar no botão em destaque “Ranking de Usuários” demonstrado abaixo 
O usuário será redirecionado para a página de ranking contendo os 10 primeiros usuários, onde os 3 primeiros recebem um destaque especial:

User Story: Visualizar pontos e troféus de usuário
Na página inicial, o usuário poderá clicar no botão destacado na imagem abaixo para acessar o seu perfil, cujo conteúdo contém os pontos e troféus

4. Modelagem e Diagramação [Disponível no doc PDF]

5.  Planejamento da Iteração

Semana 1:
Desenvolvimento front-end e interações de login (Estimado: 4 dias)
Lista completa de Livros – Front-end (Estimado: 1 dia)
Página de Livros específicos – Front-end (Estimado: 1 dia)
Ranking de usuários – Front-end (Estimado: 1 dia)

Semana 2:
Desenvolvimento do sistema de pontuação (Estimado: 4 dias)
Integração dos pontos ao perfil e interações com o ranking (Estimado: 2 dias)
Desenvolvimento do sistema de recompensa por troféus a cada 5 livros lidos do mesmo gênero (Estimado: 1 dia)

5.  Burndown Chat
As tasks representadas neste gráfico foram determinadas por possuírem a mesma estimativa de duração (4 dias). O desenvolvimento front-end e integrações de login está representado pela cor laranja no gráfico, enquanto o Desenvolvimento completo do sistema de pontuação está representado pela cor azul. Os eixos X e Y representam o sistema padrão do Burndown Chart, onde o eixo X representa os dias corridos, e o eixo Y representa o trabalho faltante para a conclusão. Neste caso em específico, o desenvolvimento do login correspondeu aos 4 dias conforme estimado. Porém, o desenvolvimento do sistema completo de pontuação ultrapassou o tempo estimado.
 
