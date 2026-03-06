
# 🧩 Padrões de Commit, Branch e Pull Request

Este documento define as convenções utilizadas para manter o histórico do projeto limpo, consistente e colaborativo.

---

## 📑 Sumário
- [Commits](#-commits)
- [Branches](#-branches)
- [Pull Requests](#-pull-requests)
- [Conclusão](#-conclusão)

---

## 📝 Commits

### Formato
Os commits devem seguir o padrão:

```
tipo: descrição da mudança
```

A descrição pode ser escrita em **PascalCase**, **camelCase**, **kebab-case** ou **snake_case**, dependendo do contexto.

### 🔖 Tipos de Commits
-  **feat:** nova funcionalidade ou adição ao projeto  
-  **fix:** correção de bugs ou erros  
-  **docs:** mudanças na documentação (ex: README.md)  
-  **assets:** adição de imagens, fontes, ícones etc.  
-  **style:** mudanças de estilo (CSS, variáveis, formatação)  
-  **refactor:** refatoração de código sem correção de bugs ou novas features  
-  **chore:** mudanças estruturais (dependências, configurações)  
-  **test:** adição ou modificação de testes  
-  **wip:** work in progress — código em andamento  

### 💡 Exemplos
```
feat: created main page
assets: added new images & svg
docs: updated README.md
```

---

## 🌿 Branches

Ao criar algo novo, sempre separe em uma branch.  
Use **camelCase** para os nomes.

###  Tipos de Branches
-  **feat/** → criação de novas funcionalidades (componentes, páginas, features)  
-  **fix/** → correção de bugs  
-  **docs/** → alterações na documentação  
-  **refactor/** → refatoração de código  
-  **chore/** → mudanças estruturais (dependências, configs)  

### 💡 Exemplos
```
feat/createdLeftSideBar
feat/createdNewsPage
chore/updatedProjectStructure
```

📸 Exemplo visual:
```
Branch: feat/createdNewsPage
PR:     [FEAT] Created News Page
```

---

## 🔁 Pull Requests (PRs)

As Pull Requests também devem seguir um padrão.  
A diferença é que o tipo vem entre **colchetes [ ]** e o título pode conter espaços.

### 🔖 Tipos de PRs
-  **[FEAT] Created ...** → nova funcionalidade ou adição completa  
-  **[CHORE] Updated ...** → alterações estruturais  
-  **[FIX] Something ...** → correções significativas  
-  **[REFACTOR] Something ...** → refatoração do projeto  

### 💡 Exemplo de diferença
| Tipo   | Exemplo                  |
|--------|--------------------------|
| Branch | `feat/createdNewsPage`   |
| PR     | `[FEAT] Created News Page` |

---

## ✅ Conclusão

Seguindo essas convenções de **Commit, Branch e Pull Request**, o projeto mantém um histórico claro, organizado e fácil de colaborar.
