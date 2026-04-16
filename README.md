# Sistema de Gerenciamento de Serviços de TI e Controle de Ativos (SGDB) 🚀

![Status do Projeto](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)
![Database](https://img.shields.io/badge/Database-PostgreSQL-blue)
![Tech](https://img.shields.io/badge/Tech-JavaScript_/_Node.js-orange)

Este projeto propõe o desenvolvimento de um banco de dados relacional robusto para suportar uma aplicação integrada de **Service Desk** e **Gestão de Inventário de TI**. O objetivo é centralizar o ciclo de vida de chamados e o controle físico/lógico de ativos, mitigando gargalos operacionais e garantindo conformidade com SLAs.

---

## 🛠️ Tecnologias Utilizadas

* **Banco de Dados:** PostgreSQL
* **Linguagem Principal:** JavaScript
* **Modelagem:** BrModel / Draw.io (DER/MER)
* **Documentação:** Dicionário de Dados Estruturado

---

## 📋 Cenário e Problema

No cenário corporativo atual, a falta de controle centralizado sobre o parque tecnológico gera:
* Tempo de inatividade prolongado.
* Dificuldade no cumprimento de SLAs.
* Perda de rastreabilidade de custos e subutilização de hardware/software.

**Nossa Solução:** Uma base de dados integrada que conecta usuários, setores, ativos (hardware/software), licenças e o histórico de manutenções/chamados em um único ecossistema.

---

## 📐 Estrutura do Projeto

### 1. Modelagem de Dados
O projeto segue as etapas de normalização e modelagem relacional, garantindo integridade e performance.

* **Entidades Principais:** `Usuario`, `Hardware`, `Software`, `Chamado`, `Manutencao`.
* **Relacionamentos:** Gestão de licenças por fornecedor, controle de estoque e alocação de patrimônio por unidade.

### 2. Dicionário de Dados
A documentação técnica detalhada (campos, tipos, chaves PK/FK e restrições) pode ser encontrada nos arquivos CSV anexados ou diretamente no `Relatório Completo.docx`.

| Tabela | Descrição |
| :--- | :--- |
| **Usuario** | Cadastro de colaboradores e vínculo com setores. |
| **Hardware** | Registro técnico de equipamentos e números de série. |
| **Software** | Gestão de versões e vínculos com licenças. |
| **Chamado** | Histórico de suporte, operadores e prazos. |
| **Estoque** | Controle quantitativo e localização física (Guarda). |

---

## 🚀 Como Executar

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/Augusto05/projeto-sgdb.git](https://github.com/Augusto05/projeto-sgdb.git)
    ```
2.  **Importe o Banco de Dados:**
    * Execute o script DDL (disponível na pasta `/sql`) no seu gerenciador PostgreSQL.
3.  **Configuração da Aplicação:**
    * (Em breve: Instruções para conexão via JavaScript/PDO).

---

## 👥 Integrantes

* **Augusto Bueno**
* **Davi Galvani**
* **João Scheffer**

---

## 🎓 Contexto Acadêmico
Projeto desenvolvido para o curso de **Tecnologia em Banco de Dados** na **Fatec Bauru**.
