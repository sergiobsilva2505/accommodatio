# Accomodatio

### Estudo de caso sobre aplicação Spring MVC com Thymeleaf

#### Tecnologias utilizadas

 - Java16
 - Maven
 - Spring Framework
   - Data Jpa
   - Boot
   - MVC
 - H2 database (somente testes)
 - JUnit
 - Mockito

### Obetivos

Desenvolver uma aplicação web utilizando Spring MVC, dentro dos requisitos realcionados abaixo:

- A aplicação de ver ter um módulo de atendimento, acessado somente pelos funcionários do hotel para execução de tarefas
diárias, como cadastro de hóspedes e reserva de apartamentos.
- A aplicação de ve ter um módulo de gerenciamento, o qual permite ao gerente do hotel executar operações de cadastro de
usuários e também executar alterações nas configurações de cada apartamento pertencente ao hotel que ele gerencia. 
- Aleḿ dos módulos de administração do hotel, restrito ao uso interno por seus funcionários e gerentes, a aplicação deve
conter ainda um módulo público, acessível a qualquer usuário que navegue na internet. Esse é o site do hotel.
- Por meio desse site, o hóspede pode consultar o hóspede pode consultar apartamento disponiveis, de acordo com as
especificaçõesque ele fornecer. Ao se decidir o usuário/hóspede pode efetuar uma reserva.
- O usuário pode visualizar seu histórico de estadia no hotel.

<br>

 _Tabela 1 - Lista de funcionalidades dos módulos de atendimento e gerencia._

| Funcionalidade | Descrição | Público-alvo |
| ------------------------ | ------------------------------------------------------------------------ | --------- |
| Cadastro de usuários | Inclusão e alteração de dados de usuários | Gerente |
| Edição de apartamentos | Alteração nas características e configurações dos apartamentos | Gerente |
| Consulta de apartamentos | Pesquisa dos apartamentos disponíveis para reserva no período. | Atendente |
| Cadastro de hóspede | Inclusão de novos hóspedes e alteração de dados cadastrais dos já existentes. | Atendente |
| Resistro de reserva | Registro efetivo de uma reserva de apartamento pelo hóspede  | Atendente |

<br>

_Tabela 2 - Lista de funcionalidades do módulo de acesso público._

| Funcionalidade | Descrição | Público-alvo   |
| -------------- | ----------| -------------- |
| Cadastro de hóspedes | Inclusão e alteração de hóspede | Usuário |
| Consulta de apartamentos | Pesquisa de apartamentos disponíveis para reserva no período e nas configurações desejadas pelo hóspede, em qualquer hotel pertencente a rede. | Usuário |
| Reserva | Registro de uma reserva de apartamento pelo hóspede. | Usuário |
| Histório de estadias | Visualização das estadias já registradas pelo hóspede na rede de hotéis. | Usuário |