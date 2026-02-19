# 📚 Editorial SaaS Ecosystem

Plataforma editorial completa composta por **API central + 3 aplicações independentes**:

- 👑 Admin (gestão estratégica)
- 👥 Colaborador (produção editorial)
- 🛍️ Cliente (consumo e compras)

Sistema desenvolvido para editora real, cobrindo todo o ciclo:

**gestão → produção → publicação → venda → acesso digital**

---

## 🔒 Status do projeto

Projeto finalizado para cliente real, porém descontinuado antes do lançamento em produção.

Por se tratar de software proprietário, o código-fonte não é público.

📩 Recrutadores podem solicitar:
- acesso ao repositório privado  
- demonstração guiada  
- apresentação técnica  

---

# ⚙️ Backend API (Arquitetura Hexagonal)

API central construída em **Arquitetura Hexagonal (Ports & Adapters)**, com domínio isolado de frameworks.

**Responsabilidades principais:**

- autenticação e RBAC  
- gestão editorial  
- publicações digitais  
- vendas e acesso do cliente  
- integração entre aplicações  

Tecnologias: Node.js, TypeScript, Prisma, Redis, Tsyringe.

### 🏗️ Estrutura e Arquitetura

<table>
  <tr>
    <td align="center"><img src="assets/editora/api/1.png" height="220"></td>
    <td align="center"><img src="assets/editora/api/2.png" height="220"></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/editora/api/3.png" height="220"></td>
    <td align="center"><img src="assets/editora/api/4.png" height="220"></td>
  </tr>
</table>

---

# 🛡️ Infraestrutura & DevOps

Ecossistema totalmente containerizado com Docker e orquestrado via Docker Compose.

**Ambiente:**

- VPS Linux  
- Nginx reverse proxy  
- SSL  
- containers isolados  
- deploy full-cycle  

<table>
  <tr>
    <td align="center"><img src="assets/editora/infra/1.png" height="200"></td>
    <td align="center"><img src="assets/editora/infra/2.png" height="200"></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/editora/infra/3.png" height="200"></td>
    <td align="center"><img src="assets/editora/infra/4.png" height="200"></td>
  </tr>
</table>

---

# 👑 Admin Panel

Painel estratégico para administradores da editora.

**Funcionalidades:**

- gestão de usuários e permissões (RBAC)  
- controle de conteúdos  
- visão global do sistema  
- métricas editoriais  

<table>
  <tr>
    <td align="center"><img src="assets/editora/admin/1.png" height="240"></td>
    <td align="center"><img src="assets/editora/admin/2.png" height="240"></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/editora/admin/3.png" height="240"></td>
    <td align="center"><img src="assets/editora/admin/4.png" height="240"></td>
  </tr>
</table>

---

# 👥 Employee Dashboard

Interface operacional para colaboradores editoriais.

**Fluxo de trabalho:**

- criação e edição de conteúdos  
- gestão de ativos  
- organização de publicações  
- interação segura com API  

<table>
  <tr>
    <td align="center"><img src="assets/editora/employee/1.png" height="240"></td>
    <td align="center"><img src="assets/editora/employee/2.png" height="240"></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/editora/employee/3.png" height="240"></td>
    <td align="center"><img src="assets/editora/employee/4.png" height="240"></td>
  </tr>
</table>

---

# 🛍️ Client Storefront

Aplicação pública voltada ao leitor final.

**Funcionalidades:**

- vitrine de publicações  
- autenticação de clientes  
- biblioteca digital  
- experiência otimizada para SEO  

<table>
  <tr>
    <td align="center"><img src="assets/editora/client/1.png" height="240"></td>
    <td align="center"><img src="assets/editora/client/2.png" height="240"></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/editora/client/3.png" height="240"></td>
    <td align="center"><img src="assets/editora/client/4.png" height="240"></td>
  </tr>
</table>

---

# 🛠️ Stack Tecnológica

| Camada | Tecnologias |
|--------|------------|
Backend | Node.js, TypeScript, Express, Prisma, Redis, Tsyringe |
Frontend | Next.js, Next Auth, Chakra UI, Tailwind |
Infra | Docker, Docker Compose, Nginx, Linux VPS, SSL |

---

# 👤 Autor

**Tiago R. Becker**  
Desenvolvedor Fullstack especializado em arquitetura escalável e engenharia full-cycle.
