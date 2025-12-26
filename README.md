# 🧪 Casos de Teste – Login e Cadastro

## 📌 Sobre o Projeto
Este repositório contém a **documentação de casos de teste funcionais** das funcionalidades de **Login e Cadastro** de um sistema web.

O objetivo é demonstrar, de forma organizada e profissional, a modelagem de cenários de teste contemplando:
- Fluxos positivos
- Fluxos negativos
- Validações de segurança
- Usabilidade
- Regras de negócio

O material foi elaborado seguindo boas práticas de **QA Manual**, utilizando:
- Casos de teste estruturados
- Pré-condições claras
- Passos comuns reutilizáveis
- Resultados esperados bem definidos

---

## 🎯 Objetivo Geral
Garantir que as funcionalidades de **Cadastro e Login**:
- Funcionem corretamente
- Bloqueiem entradas inválidas
- Tratem duplicidade de dados
- Forneçam feedback claro ao usuário
- Redirecionem corretamente em fluxos de sucesso

---

## 📂 Estrutura dos Testes

As funcionalidades testadas estão organizadas em **8 cenários principais**:

1. Cadastro com campos obrigatórios vazios  
2. Cadastro com campos inválidos  
3. Cadastro com dados já existentes (duplicidade)  
4. Cadastro com dados válidos  
5. Login com campos obrigatórios vazios  
6. Login com dados inválidos ou inexistentes  
7. Funcionamento do botão **"Esqueceu a senha"**  
8. Login com credenciais válidas  

Cada cenário contém:
- Objetivo do teste  
- Pré-condições  
- Passos de execução  
- Resultado esperado  

---

## 🔁 Passos Comuns (PCs)

Para evitar repetição excessiva e facilitar a manutenção, foram definidos **Passos Comuns** reutilizáveis:

- **PC-01** – Acessar a página correspondente (Login ou Cadastro)  
- **PC-02** – Preencher corretamente os campos não relacionados ao cenário  
- **PC-03** – Submeter o formulário  

Esses passos são referenciados dentro dos casos de teste sempre que aplicável.

---

## 🧠 Boas Práticas Aplicadas
- Separação clara entre **ação**, **condição** e **resultado**
- Uso correto de **pré-condições** (estado do sistema)
- Linguagem objetiva e compreensível
- Foco em experiência do usuário (UX)
- Estrutura compatível com documentação real de QA

---

## 🛠️ Tipo de Teste
- Testes Funcionais
- Testes Manuais
- Testes de Validação de Campos
- Testes de Regras de Negócio

---

## 📎 Observações
Este projeto tem caráter **educacional e demonstrativo**, com foco em:
- Portfólio de QA
- Estudo de modelagem de casos de teste
- Organização e clareza na documentação

Pode ser facilmente adaptado para ferramentas como:
- TestRail
- Zephyr
- Jira
- Notion
- Planilhas de teste

---

## 👨‍💻 Autor
**Pedro Lucas**  
Estudante e entusiasta de **Qualidade de Software (QA)**  
Foco em testes manuais, documentação e melhoria contínua da qualidade.

---

🚀 *“Testar não é encontrar defeitos, é garantir valor.”*
