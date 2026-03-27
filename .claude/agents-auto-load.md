# Auto-Load Agentes AIOX

Este arquivo carrega automaticamente TODOS os agentes do Synkra AIOX ao abrir o repositório no Claude.

## 🚀 Agentes Disponíveis

### Ativação Rápida
Use qualquer um destes aliases para ativar o agente correspondente:

#### Desenvolvimento
- **@architect** - Arquiteto de Soluções (Aria)
  - Foco: Arquitetura, design técnico, decisões estruturais
  - Diretórios: `docs/architecture/`, system design  
  
- **@dev** - Desenvolvedor (Dex)
  - Foco: Implementação de código, features, bugs
  - Diretórios: `packages/`, `.aiox-core/core/`, `bin/`

- **@devops** - DevOps Engineer (Gage)
  - Foco: CI/CD, infraestrutura, git operations
  - Diretórios: `.github/`, deployment, push authority (EXCLUSIVO)
  - ⚠️ AUTORIDADE EXCLUSIVA para fazer push no remote

#### Qualidade
- **@qa** - QA Engineer (Quinn)
  - Foco: Testes, qualidade, cobertura de testes
  - Diretórios: `tests/`, `*.test.js`, quality gates

- **@analyst** - Analista (Alex)
  - Foco: Pesquisa, análise, dados, insights
  - Diretórios: Análise de código, documentação técnica

#### Dados & UX
- **@data-engineer** - Engenheiro de Dados (Dara)
  - Foco: Database design, migrations, schema
  - Diretórios: `packages/db/`, data layer

- **@ux-design-expert** - UX/UI Designer (Uma)
  - Foco: Design UX/UI, user experience, interfaces
  - Diretórios: Componentes de UI, design systems

#### Gestão
- **@pm** - Product Manager (Morgan)
  - Foco: Product strategy, roadmap, prioritization  
  
- **@po** - Product Owner (Pax)
  - Foco: Stories, epics, requirements, acceptance criteria
  - Diretórios: `docs/stories/`, requirements  
  
- **@sm** - Scrum Master (River)
  - Foco: Facilitação, ceremonies, blockers

#### Orquestração
- **@squad-creator** - Squad Creator
  - Foco: Criação e gerenciamento de squads

- **@aiox-master** - AIOX Master (Orquestrador)
  - Foco: Orquestração geral, koordinação entre agentes
  - Escopo: Visão macro do projeto

---

## 📋 Comandos de Agentes

Após ativar um agente com `@agent-name`, use estes comandos:

| Comando | Descrição |
|---------|-----------|
| `*help` | Mostrar comandos disponíveis do agente |
| `*create-story` | Criar nova development story |
| `*task {name}` | Executar task específica |
| `*exit` | Sair do modo agente |

---

## 🔄 Workflow Padrão

```
1. @po *create-story        # Product Owner cria story
2. @architect                # Arquiteto revisa/propõe arquitetura
3. @dev                      # Desenvolvedor implementa
4. @qa                       # QA executa testes
5. @devops push             # DevOps faz push para remote
```

---

## 📁 Localização dos Agentes

Todos os agentes estão definidos em:
**`.aiox-core/development/agents/`**

Estrutura:
```
.aiox-core/development/agents/
├── architect.md
├── dev.md
├── devops.md
├── qa.md
├── analyst.md
├── pm.md
├── po.md
├── sm.md
├── ux-design-expert.md
├── data-engineer.md
├── squad-creator.md
└── aiox-master.md
```

---

## ⚡ Quick Start

1. **Digite qualquer @ mention:**
   ```
   @dev
   ```

2. **O agente se ativa automaticamente com sua persona**

3. **Use `*help` para ver todos os comandos:**
   ```
   *help
   ```

4. **Saia com:**
   ```
   *exit
   ```

---

## 🎯 Dicas de Uso

✅ **DO:**
- Use o agente correto para a tarefa (ex: @qa para testes)
- Sempre siga stories do @po
- @devops é o ÚNICO que pode fazer push
- Mantenha atualizado o progresso das stories

❌ **DON'T:**
- Misture responsabilidades de agentes
- Tente fazer push com outro agente que não @devops
- Ignore o workflow de story-driven development

---

*Synkra AIOX - Agentes Auto-Load v4.0*
*CLI First | Observability Second | UI Third*