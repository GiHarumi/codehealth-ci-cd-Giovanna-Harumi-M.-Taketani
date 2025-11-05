# codehealth-ci-cd-Giovanna-Harumi, Rodrigo


#  CodeHealth – Pipeline de CI/CD

## 📘 Descrição
Projeto acadêmico que simula um pipeline de Integração e Entrega Contínua (CI/CD) utilizando GitHub Actions.  
O sistema representa um protótipo de **agendamento médico** da startup fictícia *CodeHealth*.

---

## ⚙️ Estrutura do Pipeline

| Etapa | Descrição |
|-------|------------|
| **Build** | Simula a compilação do projeto. |
| **Testes** | Executa validações e simula testes automáticos. |
| **Deploy (Homologação)** | Gera um artefato `.zip` se os testes passarem. |

**Gatilho:**  
O pipeline é executado automaticamente a cada `push` na branch `develop`.

---

## 🌿 Estrutura de Branches

- **main:** produção (estável)
- **develop:** integração
- **feature/teste-ci:** desenvolvimento e testes

---

## 🔒 Boas Práticas de Segurança

- O arquivo `config.env` contém variáveis sensíveis (ex.: credenciais) e **não deve ser versionado**.
- Utilizamos `.gitignore` para evitar expor dados privados.
- Secrets simulados (ex.: `DEPLOY_KEY`) são armazenados de forma segura no GitHub Secrets.

---



## 💭 Reflexão

**1. Principal vantagem da Integração Contínua para o trabalho em equipe:**  
Facilita a colaboração e reduz falhas de integração, garantindo que todos trabalhem sobre uma base de código sempre funcional e testada.

**2. Riscos de negligenciar a Gerência de Configuração:**  
Podem surgir conflitos de código, perda de versões, falhas em produção e dificuldade em rastrear mudanças.

**3. Como a automação aumenta a segurança das entregas:**  
Automatizar reduz erros humanos, garante testes consistentes e impede que código com falhas seja implantado.

---
