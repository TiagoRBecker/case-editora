Plataforma Editorial Multi-Aplicação (Case)

Sistema completo para gestão editorial composto por múltiplas aplicações integradas, incluindo API backend, painel administrativo, portal do cliente e aplicação operacional interna.

O projeto foi desenvolvido com foco em escalabilidade, separação de responsabilidades e manutenibilidade, utilizando arquitetura hexagonal e injeção de dependências.

⚠️ O código-fonte deste projeto permanece privado por confidencialidade contratual.
Este repositório apresenta a arquitetura, decisões técnicas e visão geral do sistema.

Arquitetura

O backend foi estruturado seguindo arquitetura hexagonal (Ports and Adapters), isolando completamente as regras de negócio das camadas de infraestrutura e interface.

Camadas principais:

Domain — entidades e regras de negócio

Application — casos de uso

Infrastructure — banco de dados e integrações

HTTP — controllers e rotas

DI Container — injeção de dependências com Tsyringe

Essa abordagem permite:

baixo acoplamento

alta testabilidade

facilidade de evolução

independência de frameworks

Aplicações do Ecossistema

O sistema é composto por quatro aplicações independentes:

API — backend central e regras de negócio

Admin — painel administrativo

Client — portal do cliente

Employee — aplicação operacional interna

Todas consomem a mesma API, garantindo consistência e centralização das regras.

Stack Tecnológica
Backend

Node.js

Express

TypeScript

Tsyringe (DI)

Prisma ORM

Banco relacional

Arquitetura Hexagonal

Frontend

Next.js

React

Tailwind CSS / Chakra UI

Funcionalidades Principais

Autenticação e controle de acesso

Gestão editorial

Gerenciamento de conteúdos

Painel administrativo

Portal do cliente

Fluxos operacionais internos

Integração entre múltiplas aplicações

Decisões Técnicas Relevantes

Arquitetura hexagonal para isolamento de domínio

Injeção de dependências para desacoplamento

Separação por módulos de negócio

Backend centralizado para múltiplos clientes

Camada de aplicação independente de framework

Aprendizados Técnicos

Modelagem de domínio editorial

Estruturação de backend escalável em Node.js

Organização de monorepo multi-aplicação

Aplicação prática de Ports and Adapters

Gestão de dependências em TypeScript

Autor

Tiago Becker
Desenvolvedor Backend / Fullstack
