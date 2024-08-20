**Estrutura**

Atores: 
- Administrador de TI: Configuração e manutenção do sistema e gerenciamento de permissões e acessos dos usuários.
- Suporte Técnico: Auxilia na resolução de problemas e gestão de chamados de suporte. 
- Usuário Final: Realiza tarefas diárias no sistema (acessa recursos e reporta problemas).
- Banco de dados: Armazena as informações do sistema.

**Casos de Uso**

- Administrador de TI: Configura Hardware/Software, Estabelece políticas de segurança e gerenciamento, Gerencia usuários, Monitora performance, Gerencia backups, Atualiza o sistema.
- Suporte Técnico: Gerencia chamados, Diagnóstico de problemas, Mantém registros de problemas. 
- Usuário Final: Acessa recursos, Reporta problemas, Consulta documentação.
- Banco de dados: Armazenar dados, Consultar dados, Atualizar Dados, Excluir dados.

**Diagrama de Classes**

  Usuário - Atributos
- id: int
- nome: string
- email: string
- senha: string
- tipo: string
  Usuário - Métodos
- login():boolean
- alterarSenha(nova senha: string): void
- consultarDocumentacao(): void

  Administrador(Herda Usuário) - Atributos
- permissoes: List<string>
  Administrador(Herda Usuário) - Métodos
- configurarSistema(configuracao: Configuracao): void
- gerenciarUsuarios(usuario: Usuario, acao: string): void
- monitorarPerformance(): PerformanceRelatorio
- gerenciarBackups(acao: string): void
- atualizarSistema(): void

  Usuário Final (Herda de Usuário) - Métodos
- reportarProblema(problema: Problema): void
- acessarRecursos(): void

  Suporte Técnico (Herda de Usuários) - Métodos
- gerenciarTickets(ticket: Ticket, acao: string): void
- diagnosticarProblema(problema: Problema): void
- manterRegistros(incidente: Incidente): void
