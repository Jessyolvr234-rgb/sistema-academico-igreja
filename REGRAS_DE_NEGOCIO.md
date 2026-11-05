# REGRAS DE NEGÓCIO
## Sistema Acadêmico do Curso de Crescimento Cristão — CCC

**Documento:** Regras de Negócio  
**Versão:** 1.0  
**Status:** Em planejamento  
**Última atualização:** Novembro de 2026

---

## 1. Objetivo

Este documento define as regras que controlam o funcionamento acadêmico e administrativo do Sistema CCC.

As regras deverão ser aplicadas independentemente da interface utilizada, garantindo consistência entre as operações realizadas pelos alunos, professores, coordenadores e administradores.

## 2. RN — Cadastro e acesso

### RN001 — Cadastro de usuário
O sistema deverá permitir que visitantes realizem cadastro na plataforma.

### RN002 — Aprovação obrigatória
A criação de uma conta não concede automaticamente acesso à área acadêmica. Toda solicitação deverá passar por análise administrativa.

### RN003 — Status da solicitação
Uma solicitação de acesso deverá possuir um dos seguintes status:
- Pendente;
- Aprovada;
- Rejeitada.

### RN004 — Acesso restrito
Somente usuários com acesso aprovado poderão utilizar as funcionalidades da área acadêmica.

### RN005 — Rejeição
Quando uma solicitação for rejeitada, o administrador poderá informar um motivo. O usuário deverá conseguir consultar o status e, quando disponível, o motivo da rejeição.

### RN006 — Separação entre acesso e matrícula
A aprovação do acesso à plataforma não representa matrícula automática em um curso.

O sistema deverá tratar separadamente:
- Conta de usuário;
- Aprovação de acesso;
- Solicitação de matrícula;
- Matrícula aprovada.

## 3. RN — Cursos e turmas

### RN007 — Cursos iniciais
A primeira versão deverá disponibilizar:
- CCC1 — Curso de Crescimento Cristão 1;
- CCC2 — Curso de Crescimento Cristão 2.

### RN008 — Uma turma por curso
Na versão inicial, cada curso deverá possuir apenas uma turma.

A estrutura técnica deverá permitir a expansão para várias turmas futuramente.

### RN009 — Modalidade
As aulas serão realizadas exclusivamente na modalidade online.

### RN010 — Configuração de curso
Cada curso deverá possuir informações como:
- Nome;
- Descrição;
- Situação;
- Valor, quando aplicável;
- Pré-requisitos;
- Critérios de conclusão;
- Configurações de certificação.

### RN011 — Situação do curso
Um curso poderá estar disponível, em andamento, concluído ou inativo, conforme os estados definidos na implementação.

## 4. RN — Pré-requisitos e matrículas

### RN012 — Pré-requisito do CCC2
Para ingressar no CCC2, o aluno deverá ter concluído o CCC1.

### RN013 — Validação do pré-requisito
O sistema deverá verificar a conclusão do CCC1 antes de permitir a matrícula no CCC2.

### RN014 — Aprovação da matrícula no CCC2
Mesmo quando o aluno cumprir o pré-requisito, a matrícula no CCC2 dependerá de aprovação do coordenador ou administrador.

### RN015 — Matrícula independente
A aprovação de acesso à plataforma não deverá gerar matrícula automática em CCC1 ou CCC2.

### RN016 — Histórico acadêmico
O sistema deverá preservar o histórico de matrículas e conclusões, mesmo quando o aluno deixar de participar de uma turma.

## 5. RN — Disciplinas e professores

### RN017 — Disciplinas por curso
Cada curso poderá possuir várias disciplinas.

### RN018 — Aulas por disciplina
Cada disciplina poderá possuir várias aulas, organizadas em uma sequência definida.

### RN019 — Professor responsável
Cada disciplina vinculada à turma deverá possuir um professor responsável.

### RN020 — Acesso do professor
O professor deverá visualizar e acompanhar somente as disciplinas e informações permitidas por suas atribuições.

## 6. RN — Aulas e liberação de conteúdo

### RN021 — Liberação sequencial
As aulas deverão ser disponibilizadas em ordem sequencial.

### RN022 — Bloqueio da próxima aula
O aluno não poderá acessar a próxima aula enquanto não cumprir o critério de conclusão da aula anterior.

### RN023 — Critério de conclusão
O sistema deverá considerar o percentual mínimo de visualização da gravação configurado para determinar a conclusão de uma aula gravada.

O percentual ainda será definido pela administração.

### RN024 — Conteúdos de apoio
Materiais complementares poderão ser vinculados às aulas e disponibilizados aos alunos autorizados.

### RN025 — Acesso às gravações
As gravações deverão ficar disponíveis para revisão, respeitando as permissões e o período de acesso configurado.

## 7. RN — Aulas ao vivo e frequência

### RN026 — Agendamento
As aulas ao vivo deverão possuir data e horário previamente definidos.

### RN027 — Registro de participação
A frequência deverá ser calculada com base em eventos confiáveis enviados pelo provedor de videoconferência.

### RN028 — Entrada e saída
O sistema deverá considerar os horários de entrada e saída dos participantes para calcular o tempo de participação.

### RN029 — Validação dos eventos
Eventos recebidos deverão ser validados pelo servidor. O sistema não deverá confiar exclusivamente em informações enviadas pelo navegador do aluno.

### RN030 — Consolidação de frequência
Os eventos de participação deverão ser consolidados em um registro de frequência por aluno e sessão.

### RN031 — Gravação não substitui presença
Assistir posteriormente à gravação não deverá alterar automaticamente a frequência da aula ao vivo.

O progresso da gravação e a presença na aula ao vivo são registros independentes.

### RN032 — Percentual mínimo
O percentual mínimo de frequência necessário para conclusão deverá ser configurável.

### RN033 — Ausências justificadas
O sistema poderá registrar justificativas de ausência. O efeito dessas justificativas sobre o cálculo de frequência dependerá de uma política administrativa ainda a ser definida.

## 8. RN — Pagamentos

### RN034 — Curso gratuito ou pago
Cada curso ou oferta de turma deverá permitir configuração de modalidade gratuita ou paga.

### RN035 — Registro financeiro
Quando houver cobrança, o sistema deverá registrar valores, vencimentos e situação dos pagamentos.

### RN036 — Confirmação de pagamento
A confirmação de pagamentos realizados por meio de gateway deverá ocorrer mediante validação segura do retorno do provedor.

### RN037 — Histórico financeiro
O histórico financeiro deverá ser preservado para consulta pelos perfis autorizados.

### RN038 — Política financeira
Regras de parcelamento, cancelamento, reembolso, atraso e bloqueio de acesso deverão ser definidas antes da implementação financeira definitiva.

## 9. RN — Conclusão e certificados

### RN039 — Certificado por curso
O CCC1 e o CCC2 deverão possuir certificados independentes.

### RN040 — Critérios de conclusão
A emissão do certificado dependerá do cumprimento dos critérios configurados para o curso.

### RN041 — Frequência obrigatória
O aluno deverá cumprir o percentual mínimo de frequência definido para o curso.

### RN042 — Aulas obrigatórias
O aluno deverá concluir as aulas obrigatórias conforme os critérios de progresso definidos.

### RN043 — Emissão automática
Quando todos os critérios forem cumpridos, o sistema deverá registrar a conclusão e emitir o certificado automaticamente.

### RN044 — Emissão única
O sistema deverá impedir a emissão duplicada de certificados para a mesma conclusão acadêmica.

### RN045 — Histórico de certificados
Os certificados emitidos deverão permanecer disponíveis para consulta e validação.

## 10. RN — Permissões e segurança

### RN046 — Controle por perfil
Cada usuário deverá acessar somente as funcionalidades autorizadas ao seu perfil.

### RN047 — Validação no servidor
Operações administrativas e acadêmicas protegidas deverão ser validadas no servidor e no banco de dados.

### RN048 — Proteção de dados
Informações pessoais e acadêmicas deverão ser acessadas apenas por usuários autorizados.

### RN049 — Registro de ações
Ações administrativas relevantes deverão ser registradas para auditoria.

### RN050 — Integridade acadêmica
O aluno não poderá alterar diretamente sua frequência, conclusão, matrícula ou certificado.

## 11. Prioridade das regras

As regras relacionadas à autenticação, aprovação de acesso, matrícula, pré-requisitos, frequência, liberação sequencial e certificação são essenciais para a integridade do sistema.

Elas deverão ser implementadas com validação no servidor e, sempre que aplicável, restrições e políticas no banco de dados.

## 12. Decisões pendentes

As regras abaixo ainda precisam de definição formal:

- Percentual mínimo de frequência;
- Percentual de visualização para concluir uma gravação;
- Tratamento de faltas justificadas;
- Prazo de disponibilidade das gravações;
- Política de cancelamento e reembolso;
- Regras para inadimplência;
- Critérios adicionais para aprovação de matrícula;
- Política de emissão de segunda via de certificado.
