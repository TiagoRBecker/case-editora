# 📚 Editorial SaaS Ecosystem: Arquitetura Hexagonal & Engenharia Full Cycle

Este repositório documenta um ecossistema editorial de alta complexidade. O projeto foi arquitetado como uma solução escalável, composta por uma API central e três frontends independentes, utilizando práticas avançadas de engenharia de software para garantir desacoplamento e portabilidade.

> **Nota de Privacidade:** Este é um projeto proprietário e privado. Este README serve como um showcase técnico da arquitetura, decisões de design e infraestrutura implementada.

---

## ⚙️ Backend API: Core Engineering

A API foi construída sobre o padrão de **Arquitetura Hexagonal (Ports and Adapters)**. As regras de negócio residem no `Domain`, totalmente isoladas de frameworks externos. Utiliza **Tsyringe** para Injeção de Dependência, **Prisma ORM** para persistência no PostgreSQL e **Redis** para caching de alta performance.

### 🏗️ Estrutura e Arquitetura

<div align="center">
  <img src="assets/editora/api/1.png" width="300" height="300"  alt="Estrutura de Pastas">
  <img src="assets/editora/api/2.png" width="300" height="300" alt="Injeção de Dependência">
    <img src="assets/editora/api/3.png" width="300" height="300" alt="Estrutura de Pastas">
  <img src="assets/editora/api/4.png" width="300"height="300" alt="Injeção de Dependência">
</div>

---

## 🛡️ Infraestrutura & DevOps

O ecossistema é totalmente containerizado com **Docker**, garantindo que a API, os bancos de dados e os frontends rodem em ambientes isolados. O deploy foi realizado em uma **VPS Linux** própria, utilizando **Nginx** como Proxy Reverso e gerenciando certificados **SSL** para comunicação segura.

### 🐳 Orquestração e Servidor

<div align="center">
  <img src="assets/editora/infra/1.png" width="300" alt="Docker Status">
  <img src="assets/editora/infra/2.png" width="300" alt="Docker Status">
  <img src="assets/editora/infra/3.png" width="300" alt="Docker Status">
  <img src="assets/editora/infra/4.png" width="300" alt="Docker Status">
</div>

---

## 👑 Admin Panel

Interface desenvolvida em **Next.js** e **Chakra UI** para gestão de alto nível. Inclui controle de usuários (RBAC), gestão de permissões e visão estratégica de todo o sistema editorial.

### 🕹️ Interface Administrativa

<div align="center">
  <img src="assets/editora/admin/1.png" width="300" height="300" alt="Admin Dashboard">
    <img src="assets/editora/admin/2.png" width="300" height="300" alt="Admin Dashboard">
      <img src="assets/editora/admin/3.png" width="300" height="300" alt="Admin Dashboard">
        <img src="assets/editora/admin/4.png" width="300" height="300" alt="Admin Dashboard">

</div>

---

## 👥 Employee Dashboard

Módulo focado no fluxo de trabalho diário dos colaboradores. Prioriza a produtividade na gestão de conteúdos e ativos da editora, consumindo a API de forma segura e restrita.

### 🛠️ Workflow Operacional

<div align="center">
  <img src="assets/editora/employee/1.png" width="300"  height="300" alt="Listagem de Tarefas">
  <img src="assets/editora/employee/2.png" width="300" height="300" alt="Listagem de Tarefas">
  <img src="assets/editora/employee/3.png" width="300" height="300" alt="Listagem de Tarefas">
  <img src="assets/editora/employee/4.png" width="300" height="300" alt="Listagem de Tarefas">
</div>

---

## 🛍️ Client Storefront

A vitrine final para o público, focada em conversão, performance e **SEO**. Utiliza **Next Auth** para a área exclusiva do cliente e **Tailwind CSS** para um layout responsivo e veloz.

### 🌐 Experiência do Usuário

<div align="center">
  <img src="assets/editora/client/1.png" width="300" height="300" alt="Storefront Hero">
    <img src="assets/editora/client/2.png" width="300" height="300" alt="Storefront Hero">
      <img src="assets/editora/client/3.png" width="300" height="300" alt="Storefront Hero">
        <img src="assets/editora/client/4.png" width="300" height="300" alt="Storefront Hero">
</div>

---

## 🛠️ Stack Tecnológica

| Camada       | Tecnologias                                           |
| :----------- | :---------------------------------------------------- |
| **Backend**  | Node.js, TypeScript, Express, Tsyringe, Prisma, Redis |
| **Frontend** | Next.js (App Router), Next Auth, Chakra UI, Tailwind  |
| **Infra**    | Docker, Docker Compose, Nginx, Linux VPS, SSL         |

---

## 👤 Autor

**Tiago R. Becker** – Desenvolvedor Fullstack Full Cycle.
Focado em transformar regras de negócio complexas em software robusto e escalável.
