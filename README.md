 <div align="center">

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" width="72" alt="Next.js"/>

# CCC — Sistema Acadêmico

### CURSO DE CRESCIMENTO CRISTÃO

**Plataforma de gestão acadêmica e ensino cristão.**

Uma solução digital para conectar alunos, professores e administração em um ambiente acadêmico organizado, seguro e acessível.

<br/>

![Status](https://img.shields.io/badge/STATUS-PLANEJAMENTO-8B7CF6?style=for-the-badge)
![Architecture](https://img.shields.io/badge/ARCHITECTURE-MODERN-242938?style=for-the-badge)
![Platform](https://img.shields.io/badge/PLATFORM-PWA-16A085?style=for-the-badge)

</div>

---

##  Sobre o projeto

O **CCC — Sistema Acadêmico** é uma plataforma web projetada para digitalizar e centralizar a gestão do Curso de Crescimento Cristão da igreja.

O sistema contempla gerenciamento de alunos, professores, cursos, disciplinas, aulas, matrículas, frequência, pagamentos e certificados.

A proposta é oferecer uma experiência moderna, intuitiva e responsiva, com foco em segurança, automação e organização acadêmica.

##  Tech Stack

<div align="center">

### FRONTEND

<a href="https://nextjs.org/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" width="55" alt="Next.js"/></a>
&nbsp;&nbsp;
<a href="https://react.dev/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" width="55" alt="React"/></a>
&nbsp;&nbsp;
<a href="https://www.typescriptlang.org/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" width="55" alt="TypeScript"/></a>
&nbsp;&nbsp;
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="55" alt="JavaScript"/></a>

<br/>

<a href="https://developer.mozilla.org/en-US/docs/Web/HTML"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="55" alt="HTML5"/></a>
&nbsp;&nbsp;
<a href="https://developer.mozilla.org/en-US/docs/Web/CSS"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" width="55" alt="CSS3"/></a>
&nbsp;&nbsp;
<a href="https://tailwindcss.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tailwindcss/tailwindcss-original.svg" width="55" alt="Tailwind CSS"/></a>

### BACKEND & DATABASE

<a href="https://supabase.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/supabase/supabase-original.svg" width="55" alt="Supabase"/></a>
&nbsp;&nbsp;
<a href="https://www.postgresql.org/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" width="55" alt="PostgreSQL"/></a>

### DEVELOPMENT TOOLS

<a href="https://git-scm.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="55" alt="Git"/></a>
&nbsp;&nbsp;
<a href="https://github.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="55" alt="GitHub"/></a>
&nbsp;&nbsp;
<a href="https://code.visualstudio.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="55" alt="Visual Studio Code"/></a>

</div>

### Tecnologias e responsabilidades

| Tecnologia | Utilização |
|---|---|
| HTML5 + CSS3 | Estrutura e apresentação |
| JavaScript + TypeScript | Lógica e tipagem |
| React | Componentes e interfaces |
| Next.js | Framework da aplicação |
| Tailwind CSS | Estilização responsiva |
| Supabase | Backend e serviços |
| PostgreSQL | Banco de dados relacional |
| Git + GitHub | Versionamento e colaboração |

##  Principais funcionalidades

| Módulo | Descrição |
|---|---|
| Autenticação | Cadastro, login e recuperação de senha |
| Controle de acesso | Aprovação administrativa de usuários |
| Gestão de alunos | Cadastro e acompanhamento |
| Gestão de professores | Cadastro e atribuição de disciplinas |
| Cursos | Administração do CCC1 e CCC2 |
| Disciplinas | Organização acadêmica |
| Aulas | Conteúdo gravado e encontros ao vivo |
| Frequência | Registro e acompanhamento de presença |
| Progresso | Liberação sequencial de aulas |
| Financeiro | Planos, cobranças e pagamentos |
| Certificados | Emissão automática por conclusão |
| Dashboard | Indicadores e relatórios |

##  Perfis de acesso

- **Administrador:** controle geral da plataforma.
- **Coordenador:** acompanhamento e gestão acadêmica.
- **Professor:** disciplinas, aulas e alunos vinculados.
- **Aluno:** cursos, conteúdos, frequência e certificados.

##  Regras acadêmicas

- Uma turma por curso na primeira versão.
- CCC2 exige conclusão do CCC1.
- Matrícula no CCC2 mediante aprovação.
- Acesso à plataforma condicionado à aprovação administrativa.
- Aulas gravadas liberadas sequencialmente.
- Progresso calculado pelo percentual assistido.
- Frequência ao vivo validada por eventos do provedor.
- Certificados emitidos automaticamente após o cumprimento dos critérios.

##  Arquitetura

```text
                 CCC PLATFORM
                      |
              NEXT.JS + REACT
                      |
              TYPESCRIPT + CSS
                      |
               APPLICATION API
                      |
                   SUPABASE
                      |
          +-----------+-----------+
          |           |           |
         AUTH      DATABASE     STORAGE
          |       POSTGRESQL    FILES
          |
      EDGE FUNCTIONS
          |
     BUSINESS RULES
```

##  Banco de dados

**Identity & Access**
- profiles
- roles
- user_roles
- access_requests
- audit_logs

**Academic Management**
- courses
- classes
- enrollments
- subjects
- class_subjects

**Learning Management**
- lessons
- live_sessions
- recordings
- learning_materials
- lesson_progress

**Attendance**
- attendance_records
- attendance_policies
- attendance_justifications
- participation_events

**Financial Management**
- payment_plans
- invoices
- payments
- payment_receipts

**Certification & Communication**
- course_completions
- certificates
- announcements
- notifications

##  Segurança

- Supabase Authentication.
- Row Level Security (RLS).
- Controle de permissões por perfil.
- Proteção de dados conforme a LGPD.
- Validação das regras de negócio no servidor.
- Registro de ações administrativas.
- Armazenamento protegido de arquivos.
- Segredos mantidos em variáveis de ambiente.

##  Experiência e plataforma

- Design responsivo.
- Abordagem Mobile First.
- Aplicação PWA instalável.
- Interface adaptada para celular, tablet e desktop.
- Navegação por perfil de acesso.

##  Instalação

```bash
git clone URL_DO_REPOSITORIO

cd sistema-academico-ccc

npm install

npm run dev
```

A aplicação estará disponível em:

```text
http://localhost:3000
```

### Configuração do Supabase

Criar o arquivo `.env.local`:

```env
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=
```

Nunca publicar chaves privadas ou a `service_role` no frontend ou no GitHub.

##  Roadmap

- [ ] Documentação técnica
- [ ] Modelagem do banco de dados
- [ ] Configuração do Next.js
- [ ] Integração com Supabase
- [ ] Autenticação e permissões
- [ ] Gestão acadêmica
- [ ] Cursos e disciplinas
- [ ] Aulas e materiais
- [ ] Frequência e progresso
- [ ] Gestão financeira
- [ ] Certificados
- [ ] Dashboard administrativo
- [ ] Testes e validação
- [ ] Implantação

##  Status do projeto

**Em fase de planejamento e especificação técnica.**

As tecnologias apresentadas representam a stack planejada para implementação.

---

<div align="center">

# CCC

**Tecnologia, organização e propósito.**

*Uma plataforma a serviço do ensino e do crescimento cristão.*

</div>
