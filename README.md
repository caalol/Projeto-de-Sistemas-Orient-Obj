**Estrutura**

Atores: 
- Administrador de TI: Configuração e manutenção do sistema e gerenciamento de permissões e acessos dos usuários.
- Suporte Técnico: Auxilia na resolução de problemas e gestão de chamados de suporte. 
- Usuário Final: Realiza tarefas diárias no sistema (acessa recursos e reporta problemas).

**Casos de Uso**

- Administrador de TI: Configura o sistema, Estabelece políticas de segurança e gerenciamento, Gerencia usuários, Monitora performance, Gerencia backups, Atualiza o sistema.
- Suporte Técnico: Gerencia chamados, Diagnóstico de problemas, Mantém registros de problemas. 
- Usuário Final: Acessa recursos, Reporta problemas, Consulta documentação.

**Diagrama de Classes**

  Usuário - Atributos
- id: int
- nome: string
- email: string
- senha: string
  
  Usuário - Métodos
- acessarRecursos(): void
- reportarProblemas(): void
- consultarDocumentacao(): void

  Administrador - Atributos
- id: int
- nome: string
- email: string
- senha: string
- 
  Administrador - Métodos
- configurarSistema(): void
- gerenciarUsuarios(): void
- monitorarPerformance(): void
- gerenciarBackups(acao: string): void
- atualizarSistema(): void

  Suporte Técnico - Métodos
- id: string
- nome: string
- email: string
- nivel: string

  Suporte Técnico - Métodos
- gerenciarChamados(): void
- diagnosticarProblemas(): void
- manterRegistrosProblemas(): void
