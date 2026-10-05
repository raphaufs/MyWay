# MyWay

O **MyWay** é um aplicativo para organizar pacientes, agendamentos e o acompanhamento da jornada de extração de siso. Este README tem duas partes: um guia de uso para usuários e, ao final, instruções para quem precisa executar o projeto localmente.

## Guia de uso

### Acessar o aplicativo (atualmente só para Android)

1. Acesse a aba de Releases.
2. Escolha a versão que deseja usar (Idealmente a mais recente)
3. Em Assets faça o download do APK e faça a instalação em seu dispositivo
4. Solicite suas credenciais de login aos desenvolvedores.
5. Entre com o e-mail e a senha que foram entregues a você.
6. Para sair, abra o menu de opções no cabeçalho e escolha **Sair da conta**.

O acesso exige uma conta válida. O aplicativo não oferece cadastro de conta nem recuperação de senha; se você não recebeu credenciais ou não consegue entrar, fale com a pessoa responsável pelo acesso.

O MyWay precisa de conexão com a internet para carregar e atualizar as informações. O login é feito pelo Firebase e os dados das telas são consultados e alterados por um serviço remoto.

### Navegação principal

Na barra inferior, você encontrará quatro áreas:

| Área | Para que serve |
| --- | --- |
| **Agenda** | Consultar dias e horários com agendamentos e gerenciar atendimentos. |
| **Pesquisar** | Localizar pacientes e filtrar a lista por etapa da jornada. |
| **Dashboard** | Consultar o resumo da jornada de extração de siso e a distribuição por etapa. |
| **Cadastrar Paciente** | Iniciar um novo cadastro. |

### Localizar e cadastrar pacientes

Na área **Pesquisar**, digite o nome, telefone ou CPF do paciente. Use os filtros disponíveis para restringir a lista pela etapa da jornada. Toque em um resultado para abrir o perfil e consultar os dados e o acompanhamento disponíveis.

Para cadastrar alguém, abra **Cadastrar Paciente**, preencha os campos obrigatórios e salve. O formulário solicita nome, data de nascimento, CPF, telefone, endereço, número, CEP, estado, cidade e plano de tratamento. O e-mail é opcional. As opções de estado e cidade são selecionadas entre as opções exibidas no próprio formulário.

Depois do cadastro, o aplicativo confirma a operação e oferece a opção de abrir o perfil do paciente. Para alterar um cadastro existente, abra o perfil e escolha a opção de edição.

### Consultar e atualizar uma jornada

No perfil do paciente, abra a jornada para consultar as etapas e as informações registradas. O fluxo exibido contempla **Avaliação**, **Cirurgia** e **Retorno**. A conclusão representa o encerramento da jornada, não uma etapa clínica adicional.

Quando disponíveis na tela, as ações permitem registrar ou atualizar anotações, salvar alterações, avançar ou concluir uma etapa e marcar a jornada como abandonada ou reativá-la. Leia a confirmação exibida antes de concluir ou alterar o status.

Na tela da jornada também é possível selecionar imagens e documentos para associar às informações da etapa. A seleção aceita imagens PNG/JPG de até 8 MB e documentos PDF, TXT ou CSV de até 10 MB. A seleção na interface, por si só, não confirma que o arquivo ficará disponível depois; isso depende do serviço remoto.

### Usar a agenda

Na área **Agenda**, escolha uma data no calendário. Você pode alternar entre a visualização semanal e mensal; os dias com agendamentos são indicados no calendário e, ao selecionar um dia, a lista mostra os horários correspondentes.

Para criar um agendamento, use a ação de adicionar e informe paciente, data, horário e etapa da jornada. Para alterar ou excluir um compromisso, abra-o na lista e escolha a ação correspondente. O aplicativo não permite criar novos agendamentos para uma jornada marcada como abandonada.

### Consultar o dashboard

O **Dashboard** resume as jornadas de **Siso (Extração)**. Abra o resumo para consultar a distribuição por etapa e a lista de pacientes associados. O conteúdo apresentado depende dos dados retornados pelo serviço remoto.

### Quando algo não carregar

Se aparecer uma mensagem de erro ao carregar os dados, confira a conexão com a internet e use a opção de tentar novamente, quando exibida. Se o problema continuar, entre em contato com a pessoa que forneceu sua conta.
