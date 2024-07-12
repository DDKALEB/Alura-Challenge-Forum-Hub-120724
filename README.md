# Alura-Challenge-Forum-Hub-120724
Vamos usar o Spring Framework e criar um sistema de autenticação que valide se a pessoa usuária está realmente autorizada a realizar a ação que está tentando fazer.
Aqui está um resumo dos requisitos:

Criar um tópico: um usuário pode criar um novo tópico com título, nome do curso, mensagem e data de criação.
Listar tópicos: O aplicativo deve listar todos os tópicos.
Liste um único tópico: O aplicativo deve permitir que os usuários visualizem um único tópico.
Atualizar um tópico: um usuário pode atualizar um tópico, mas somente se for o autor do tópico.
Excluir um tópico: um usuário pode excluir um tópico, mas somente se for o autor do tópico.
Autenticação e autorização: A aplicação deve possuir mecanismos de autenticação e autorização para garantir que apenas usuários cadastrados e logados possam criar e gerenciar tópicos.
Leiame: O aplicativo deve ter um arquivo leiame bem construído que explique como o aplicativo funciona, as tecnologias utilizadas e os desafios enfrentados durante o desenvolvimento.
implementar a lógica de gerenciamento de usuários e tokens JWT para autenticação e autorização.

Nesse exemplo, estamos usando o Spring Security para proteger os endpoints /topics, /topics/{id} e /topics/{id} para usuários com papel "USER". Apenas usuários autenticados com papel "USER" podem acessar esses endpoints.
Aqui está um exemplo de como implementar a lógica de gerenciamento de usuários e tokens JWT para autenticação e autorização:
Nesse exemplo, estamos usando o Spring Security para implementar a autenticação e autorização. 
O serviço de autenticação (AuthService) é responsável por verificar as credenciais do usuário e gerar um token JWT se a autenticação for bem-sucedida. 
O utilitário de token JWT (JwtTokenUtil) é responsável por gerar e validar os tokens JWT. O filtro de autenticação (AuthenticationFilter) 
é responsável por verificar se o token JWT é válido e autenticar o usuário se for o caso. A configuração de segurança (SecurityConfig) 
é responsável por configurar a autenticação e autorização para os endpoints.

