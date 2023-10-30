# Projeto de Prática profissional em ADS
## Grupo: Pratica profissional
#Sistema My Tasks

My Tasks é um aplicativo de gerenciamento de tarefas, promovendo de forma pragmática e intuitiva a organização de tarefas, atividades e lembretes do usuário.

a) O aplicativo deverá permitir que o usuário gerencie seu cronograma diário, cefetuando as seguintes ações: adicionar novas tarefas, efetuar alterações nos campos descritivos e selecionar as concluídas, resultando em sua exclusão.

Para teste: 
Usuario: login
Senha: login
## 1. Descrições de Caso de Uso

# 1.1. Criar Nova Tarefa (CDU001)
**Resumo:** O usuário, deseja criar uma nova tarefa em seu aplicativo.
**Ator Principal:** Usuário
**Pré-Condições:** O usuário precisa estar autenticado no aplicativo, para que possa prosseguir com a criação da tarefa necessária.
**Pós-Condições:** A tarefa estará disponível para vizualização, após criação. 

#### Fluxo Principal

1. O usuário informa suas credenciais para autenticação;
2. O sistema reconhece as credenciais do usuário e o direciona para a interface "My Tasks" do usuário;
3. O usuário pressiona o botão "Add Task";
4. O usuário fornece as informações para a tarefa que deseja criar:
    4.1. Título da tarefa (Obrigatório);
    4.2. Descrição da Tarefa (se necessário);
    4.3. Seleção de data;
    4.4. Seleção de horário da tarefa.
4. O sistema identifica se houve preenchimento das informações obrigatórias e pertinentes a tarefa;
5. O usuário pressiona o botão "Salvar"; 
6. A tarefa é adicionada à interface do usuário.

#### Fluxo de exceção

Passo 4a - Caso o campo não tenha sido preenchido, o sistema emite um alerta solicitando preenchimento. O caso de uso retorna ao passo 3.

# 2.2. Alteração de Informações da Tarefa (CDU002)
**Resumo:** O usuário, deseja alterar uma tarefa, segundo suas expectativas.
**Ator Principal:** Usuário
**Pré-Condições:** O usuário precisa estar autenticado no aplicativo, é necessário que a tarefa tenha sido previamente criada.
**Pós-Condições:** A tarefa terá disponibilidade para seleção e alteração das informações que nela constam.

#### Fluxo de atividade de alteração

1. O usuário informa suas credenciais para autenticação;
2. O sistema reconhece as credenciais do usuário e o direciona para a interface "My Tasks" do usuário;
3. O sistema disponibiliza tarefas que foram previamente criadas na interface do usuário;
4. O usuário seleciona a tarefa que deseja ser alterar;
5. O sistema disponibiliza as informações inerentes a tarefa;
6. O usuário pode efetuar alterações nos campos:
    6.1. Título da tarefa (se necessário, alterar);
    6.2. Descrição da Tarefa (se necessário);
    6.3. Seleção de data (se necessário);
    6.4. Seleção de horário da tarefa (se necessário).
7. O sistema identificará se alterações foram efetuadas, e disponibilizará, a seleção do botão "Salvar Alterações";
8. O usuário poderá selecionar o botão "Salvar Alterações";
9. O sistema aplicará as alterações efetuadas pelo usuário e disponibilizará a visualização da tarefa alterada na interface do "My Tasks".

#### Fluxo de exceção

Passo 7a - Caso o sistema identifique que os campos não tenham sofrido alteração, a opção "Salvar Alterações" não estará disponível para seleção. O caso de uso avança para o passo 8a.

Passo 8a - Caso o usuário não efetue alterações nos campos pertinentes a tarefa, pode ser selecionada a opção "Voltar". O caso de uso retorna ao passo 3.

# 1.3. Seleção de Tarefa Concluída e Exclusão (CDU003)
**Resumo:** O usuário, deseja marcar uma tarefa que ele tenha concluído, segundo suas expectativas
**Ator Principal:** Usuário
**Pré-Condições:** O usuário precisa estar autenticado no aplicativo, é necessário que a tarefa tenha sido previamente criada e executada pelo usuário, mediante às expectativas de realização do objetivo da tarefa proposta.
**Pós-Condições:** A tarefa terá disponibilidade para seleção e alteração de parâmetro para "Tarefa Concluída".

#### Fluxo de Conclusão

1. O usuário informa suas credenciais para autenticação;
2. O sistema reconhece as credenciais do usuário e o direciona para a interface "My Tasks" do usuário;
3. O sistema disponibiliza tarefas que foram previamente criadas na interface do usuário;
4. O usuário pode selecionar uma ou mais tarefas, as quais tenha atingido objetivo proposto;
5. O sistema disponibilizará o botão "Tarefa Concluída";
6. O usuário selecionará o botão "Tarefa Concluída";
5. O sistema fará a marcação e posteriormente a exclusão das tarefas que foram previamente selecionadas.

#### Fluxo de exceção

Passo 4a - Caso o usuário desista de fazer a confirmação de conclusão e exclusão de alguma tarefa que tenha selecionado, ele pode desmarcar a tarefa. O caso de uso retorna para o passo 3.