# REQUISITOS DO SISTEMA
## Sistema Acadêmico do Curso de Crescimento Cristão — CCC

**Documento:** Levantamento de Requisitos  
**Versão:** 1.0  
**Status:** Em planejamento  
**Última atualização:** Novembro de 2026

---

## 1. Visão geral

O Sistema Acadêmico CCC tem como objetivo digitalizar e centralizar a gestão acadêmica dos cursos de Crescimento Cristão, permitindo administrar alunos, matrículas, disciplinas, aulas, professores, frequência, conteúdos, pagamentos e certificados.

A plataforma deverá oferecer uma experiência simples, organizada, segura e responsiva, atendendo às necessidades dos administradores, coordenadores, professores e alunos.

## 2. Objetivos do sistema

- Centralizar as informações acadêmicas.
- Organizar os cursos CCC1 e CCC2.
- Gerenciar solicitações de acesso e matrículas.
- Disponibilizar aulas ao vivo e gravações.
- Controlar a frequência dos alunos.
- Acompanhar o progresso nas disciplinas.
- Gerenciar pagamentos, quando aplicável.
- Emitir certificados automaticamente após o cumprimento dos requisitos.
- Facilitar a comunicação entre administração, professores e alunos.

## 3. Usuários e perfis

### 3.1 Administrador

Responsável pela administração geral da plataforma.

Requisitos:
- Gerenciar usuários e permissões.
- Aprovar ou rejeitar solicitações de acesso.
- Cadastrar e editar cursos.
- Gerenciar turmas.
- Cadastrar disciplinas e aulas.
- Vincular professores às disciplinas.
- Gerenciar matrículas.
- Configurar critérios de frequência e conclusão.
- Consultar relatórios acadêmicos e financeiros.
- Gerenciar pagamentos.
- Emitir ou consultar certificados.
- Publicar comunicados.

### 3.2 Coordenador

Responsável pelo acompanhamento acadêmico dos cursos.

Requisitos:
- Acompanhar turmas e alunos.
- Consultar frequência.
- Acompanhar o progresso acadêmico.
- Gerenciar ou validar matrículas, conforme as permissões concedidas.
- Acompanhar professores e disciplinas.
- Consultar relatórios acadêmicos.

### 3.3 Professor

Responsável pelas disciplinas vinculadas a ele.

Requisitos:
- Visualizar suas disciplinas.
- Consultar a lista de alunos.
- Visualizar o calendário de aulas.
- Consultar gravações e materiais.
- Acompanhar a participação dos alunos.
- Consultar relatórios de frequência de suas disciplinas.

### 3.4 Aluno

Responsável por acompanhar sua trajetória acadêmica.

Requisitos:
- Criar uma conta.
- Solicitar acesso à plataforma.
- Consultar o status da solicitação.
- Visualizar os cursos disponíveis.
- Acompanhar sua matrícula.
- Acessar disciplinas e aulas liberadas.
- Participar de aulas ao vivo.
- Assistir às gravações.
- Consultar sua frequência.
- Acompanhar seu progresso.
- Consultar pagamentos, quando aplicável.
- Acessar certificados emitidos.

## 4. Requisitos funcionais

Os requisitos funcionais descrevem as ações que o sistema deverá executar.

| Código | Requisito |
|---|---|
| RF001 | Permitir cadastro de usuários. |
| RF002 | Registrar solicitações de acesso à plataforma. |
| RF003 | Permitir aprovação ou rejeição de solicitações por administrador. |
| RF004 | Permitir autenticação segura de usuários. |
| RF005 | Controlar acesso conforme o perfil e as permissões. |
| RF006 | Cadastrar e gerenciar cursos. |
| RF007 | Disponibilizar CCC1 e CCC2. |
| RF008 | Gerenciar uma turma por curso na versão inicial. |
| RF009 | Cadastrar disciplinas vinculadas aos cursos. |
| RF010 | Vincular professores às disciplinas. |
| RF011 | Cadastrar aulas e materiais de apoio. |
| RF012 | Organizar a sequência de liberação das aulas. |
| RF013 | Bloquear a próxima aula enquanto a anterior não estiver concluída. |
| RF014 | Cadastrar datas e horários de aulas ao vivo. |
| RF015 | Disponibilizar links de acesso às aulas ao vivo. |
| RF016 | Armazenar ou integrar gravações das aulas. |
| RF017 | Disponibilizar gravações para revisão. |
| RF018 | Registrar eventos de entrada e saída das aulas ao vivo por integração com o provedor. |
| RF019 | Consolidar os registros de participação para calcular frequência. |
| RF020 | Permitir consulta da frequência pelo aluno. |
| RF021 | Configurar percentual mínimo de frequência. |
| RF022 | Registrar justificativas de ausência, conforme política definida. |
| RF023 | Acompanhar o progresso individual do aluno. |
| RF024 | Configurar critérios de conclusão dos cursos. |
| RF025 | Emitir certificados automaticamente quando os critérios forem cumpridos. |
| RF026 | Gerenciar pagamentos, quando o curso for pago. |
| RF027 | Consultar situação financeira do aluno. |
| RF028 | Publicar comunicados e notificações. |
| RF029 | Disponibilizar relatórios acadêmicos. |
| RF030 | Disponibilizar relatórios financeiros aos perfis autorizados. |
| RF031 | Manter histórico das principais ações administrativas. |

## 5. Requisitos não funcionais

| Código | Requisito |
|---|---|
| RNF001 | A interface deverá ser responsiva. |
| RNF002 | O desenvolvimento deverá priorizar dispositivos móveis. |
| RNF003 | O sistema deverá funcionar em navegadores modernos. |
| RNF004 | A autenticação deverá ser segura. |
| RNF005 | As permissões deverão ser verificadas no servidor e no banco de dados. |
| RNF006 | Dados pessoais deverão ser protegidos conforme a LGPD. |
| RNF007 | Senhas não deverão ser armazenadas diretamente nas tabelas da aplicação. |
| RNF008 | Arquivos privados deverão possuir controle de acesso. |
| RNF009 | O sistema deverá registrar ações administrativas relevantes. |
| RNF010 | A arquitetura deverá permitir evolução e manutenção. |
| RNF011 | O sistema deverá possuir tratamento de erros e validação de dados. |
| RNF012 | A aplicação deverá oferecer possibilidade de instalação como PWA. |
| RNF013 | Operações críticas deverão ser executadas de forma consistente e segura. |

## 6. Requisitos de interface

A interface deverá seguir os seguintes princípios:

- Design moderno e profissional.
- Navegação simples e intuitiva.
- Layout mobile-first.
- Compatibilidade com celular, tablet e computador.
- Menus adaptados ao perfil do usuário.
- Painéis com informações relevantes.
- Formulários com validação.
- Mensagens claras de sucesso, erro e pendência.
- Acessibilidade e boa legibilidade.

## 7. Fluxos principais

### 7.1 Cadastro e aprovação de acesso

1. O visitante acessa a plataforma.
2. Realiza seu cadastro.
3. O sistema cria a conta e registra uma solicitação de acesso.
4. A solicitação permanece pendente.
5. O administrador analisa os dados.
6. O administrador aprova ou rejeita a solicitação.
7. O usuário recebe a atualização do status.
8. Somente usuários aprovados podem acessar a área acadêmica.

### 7.2 Matrícula

1. O usuário aprovado visualiza os cursos disponíveis.
2. Solicita matrícula no curso desejado.
3. O sistema verifica os pré-requisitos.
4. A matrícula é submetida à aprovação quando necessário.
5. Após a aprovação, o aluno passa a ter acesso aos conteúdos liberados.

### 7.3 Acompanhamento das aulas

1. O aluno acessa sua turma.
2. Visualiza as disciplinas disponíveis.
3. Acessa a primeira aula liberada.
4. Participa da aula ao vivo ou consulta a gravação.
5. O sistema registra o progresso.
6. Após cumprir o critério de conclusão, a próxima aula é liberada.

### 7.4 Conclusão e certificação

1. O sistema verifica os requisitos de conclusão.
2. Confere a frequência mínima configurada.
3. Confere a conclusão das aulas obrigatórias.
4. Verifica outras condições acadêmicas aplicáveis.
5. Registra a conclusão do curso.
6. Emite o certificado correspondente.

## 8. Critérios gerais de aceitação

O sistema será considerado funcional quando:

- Usuários conseguirem criar contas e solicitar acesso.
- Administradores conseguirem aprovar ou rejeitar solicitações.
- Apenas usuários autorizados acessarem a área acadêmica.
- Os cursos e suas turmas puderem ser administrados.
- Disciplinas e aulas puderem ser organizadas.
- A liberação sequencial das aulas funcionar.
- As gravações puderem ser consultadas pelos alunos autorizados.
- A frequência puder ser consolidada a partir dos eventos válidos do provedor.
- O progresso acadêmico puder ser acompanhado.
- Os critérios de conclusão forem verificados corretamente.
- Os certificados forem emitidos sem duplicidade.
- As informações financeiras forem acessíveis somente a usuários autorizados.

## 9. Pendências de definição

- Provedor de videoconferência.
- Plataforma de armazenamento e reprodução de gravações.
- Percentual mínimo de frequência.
- Percentual mínimo de visualização de gravações.
- Política para faltas justificadas.
- Gateway de pagamento.
- Política de cancelamento e reembolso.
- Identidade visual definitiva dos certificados.
- Regras específicas de aprovação de matrícula no CCC1.
- Permissões detalhadas do coordenador.
