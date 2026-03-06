
# 🧭 Nomenclatura das Branches

Este documento define o padrão de nomenclatura das branches para manter o fluxo de trabalho organizado, colaborativo e sem conflitos.

---

## 📑 Sumário
- [Regras Gerais](#-regras-gerais)
- [Tipos de Branches](#-tipos-de-branches)
- [Branches Principais](#-branches-principais)
- [Fluxo Resumido](#-fluxo-resumido)
- [Conclusão](#-conclusão)

---

## 📌 Regras Gerais

- Nunca faça commits diretamente nas branches principais (`develop`, `production`).  
- Cada pessoa deve trabalhar em sua própria branch.  
- Para cada página ou funcionalidade nova, crie uma branch separada.  
- Abrevie nomes muito grandes para manter a clareza.  

### 💡 Exemplo
- Páginas: `NewsPage`, `NewsPage404`, `GamePageNoComments`  
- Branches:  
  - `feat/createdNewsPage`  
  - `feat/NewsPage404`  
  - `feat/GamePageNC`  

---

## 🌿 Tipos de Branches

### 🔹 **feat/** (nova feature)
Branches temporárias criadas para desenvolvimento de novas funcionalidades.  
São derivadas de `develop` e, após concluídas, devem ser mescladas em `develop` e depois deletadas.

### 🔹 **fix/** (correção de bug)
Criadas para corrigir problemas encontrados durante os testes.  
Exemplo: `fix/headerAlignmentBug`.

### 🔹 **docs/** (documentação)
Alterações relacionadas apenas à documentação.  
Exemplo: `docs/updateReadme`.

### 🔹 **refactor/** (refatoração)
Usadas para melhorar ou reorganizar o código sem adicionar novas funcionalidades.  
Exemplo: `refactor/apiConnection`.

### 🔹 **chore/** (mudanças estruturais)
Alterações que não afetam diretamente o código de negócio, como dependências ou configurações.  
Exemplo: `chore/updateDependencies`.

---

## 🧩 Branches Principais

### 🔹 **develop**
- Branch de integração.  
- Recebe merges das branches de desenvolvimento (`feat/`, `fix/`, etc.).  
- Nunca faça commit direto em `develop`.  

### 🔹 **production**
- Branch estável e finalizada.  
- Recebe merge apenas da `develop` após validação e testes.  
- Usada para releases e deploys em produção.  

---

## ⚙️ Fluxo Resumido

```
feat/minha-feature
        ↓
     develop
        ↓
    production
```

---

## ✅ Conclusão

Seguindo este padrão de **Naming Convention** para branches, garantimos um fluxo de trabalho organizado, seguro e colaborativo, evitando conflitos e mantendo o histórico limpo.
