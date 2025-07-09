# BlankDots

Frontend

For the frontend, you'll likely use:

JavaScript: As the primary language for client-side scripting.
TypeScript: As a superset of JavaScript, providing additional features like type checking and object-oriented programming.
React Native: As a framework for building cross-platform mobile apps.
Backend

For the backend, you'll likely use:

Java: As the primary language for server-side programming.
Firebase: As a backend-as-a-service (BaaS) platform, providing features like authentication, real-time database, and cloud functions.







Parâmetros :

Log in com email, pode-se recuperar a pass, máimo de 3 tentativas.
Pass segura contra ataque por força bruta.


Mensagens com limite máimo de 1 mês.

Gerador de ids:
- tem 1 hora de tempo limite;
- dá para cancelar;
- após gerado, é preciso ser usado ou removido para gerar outro;
- quando é aceite aparece notificação e deia escolher o nome para a conversa;
- aparece quando é tirado print;
- quando é eliminado é eliminado para os dois, mas envia notificação;


Tabelas base de dados:

Users Table
id (primary key): unique identifier for each user
email: email address of the user

Conversations Table
id (primary key): unique identifier for each conversation
user1_id (foreign key): reference to the id of the first user in the conversation
user2_id (foreign key): reference to the id of the second user in the conversation
created_at: timestamp when the conversation was created

Messages Table
id (primary key): unique identifier for each message
conversation_id (foreign key): reference to the id of the conversation that the message belongs to
user_id (foreign key): reference to the id of the user who sent the message
text: text content of the message
created_at: timestamp when the message was sent