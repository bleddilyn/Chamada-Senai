#  ChamadaSENAI

Sistema web de gerenciamento de presença e chamada online desenvolvido para o SENAI, com controle de frequência, justificativas de faltas e comunicação institucional.

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white) ![Status](https://img.shields.io/badge/status-em%20funcionamento-brightgreen)

## 👥 Equipe

**Projeto desenvolvido por 4 desenvolvedoras do SENAI:**

- **Daniele Lucena Ronquim** - Full-stack Developer  
  *(MVC Java, HTML/CSS, integração do sistema)*
- **Júlia Camilo Ribeiro** - Backend & Database Specialist  
  *(MySQL, DAOs, modelagem de banco de dados)*
- **Isabella Affonso Aldrighi** - UX/UI Designer & DevOps  
  *(Prototipagem, diagramação, edição de vídeo pitch)*
- **Helena Barioni Garcia** - Tech Lead & Documentation  
  *(Liderança técnica, documentação completa, gestão do projeto)*

**Colaboração:** Trabalho em equipe com divisão por especialidades e integração contínua.

## 🎯 Sobre o Projeto

O **ChamadaSENAI** é um sistema completo de gestão de frequência desenvolvido para atender às necessidades específicas do SENAI. A plataforma digitaliza o processo de chamada, justificativas de faltas e comunicação interna, substituindo métodos manuais e otimizando o tempo dos professores e da equipe administrativa.

### Problema Resolvido
- Eliminação de planilhas manuais e registros em papel
- Centralização das informações de frequência
- Automatização do processo de justificativas
- Comunicação eficiente entre setores

## 👥 Público-Alvo
- **Professores** do SENAI
- **Alunos** matriculados nos cursos
- **Setor de Apoio/Administrativo**

## ✨ Funcionalidades por Perfil

### 👨‍🏫 **Professor**
- ✅ Realizar chamadas online por turma
- ✅ Visualizar histórico de presença dos alunos
- ✅ Registrar observações sobre faltas
- ✅ Consultar justificativas pendentes
- ✅ Exportar relatórios de frequência

### 🎓 **Aluno**
- ✅ Justificar faltas com comprovantes
- ✅ Visualizar histórico próprio de presença
- ✅ Consultar avisos e eventos institucionais
- ✅ Acompanhar status das justificativas
- ✅ Receber notificações importantes

### 🏢 **Setor de Apoio**
- ✅ Criar e gerenciar eventos institucionais
- ✅ Publicar avisos e comunicados
- ✅ Analisar e validar justificativas de faltas
- ✅ Gerar relatórios administrativos
- ✅ Gerenciar calendário acadêmico

## 🏗️ Arquitetura do Sistema

### **Backend**
- **Linguagem:** Java
- **Servidor Web:** Apache Tomcat 9+
- **Padrão de Projeto:** MVC (Model-View-Controller)
- **Camadas:** Controller → Service → DAO → Database

### **Frontend**
- **Tecnologias:** HTML5, CSS3, JavaScript Vanilla
- **Estilização:** CSS personalizado com design institucional
- **Interatividade:** JavaScript para validações e AJAX

### **Banco de Dados**
- **SGBD:** MySQL 8.0+
- **Características:** Relacional com constraints e foreign keys
- **Backup:** Scripts de backup automático

## 🚀 Primeiros Passos

### **Pré-requisitos**
- JDK 11 ou superior
- Apache Tomcat 9+
- MySQL Server 8.0+
- Navegador web atualizado

### **Instalação do Banco de Dados**

```sql
-- 1. Criar banco de dados
CREATE DATABASE banco_cs;
USE banco_cs;

-- 2. Executar script de criação de tabelas
-- (arquivo: database/schema.sql)

-- 3. Inserir dados iniciais
-- (arquivo: database/initial_data.sql)
```

### **Configuração do Projeto**

1. **Clone o repositório:**
```bash
git clone https://github.com/julia-camilo/chamada-senai.git
cd chamada-senai
```

2. **Configure o banco de dados:**
   - Edite `src/main/resources/db.properties` com suas credenciais

3. **Compile o projeto:**
```bash
javac -cp "lib/*:." src/**/*.java -d WEB-INF/classes
```

4. **Implante no Tomcat:**
   - Copie a pasta `webapp` para `$CATALINA_HOME/webapps/`
   - Inicie o servidor Tomcat

5. **Acesse a aplicação:**
   - URL: `http://localhost:8080/chamadasenai`

### **Credenciais Padrão**
```
Professor: prof@senai.com / senha123
Aluno: aluno@senai.com / senha123
Setor Apoio: apoio@senai.com / senha123
```

## 🔒 Segurança

- **Autenticação:** Login com email e senha hash (BCrypt)
- **Autorização:** Controle de acesso por tipo de usuário
- **Sessões:** Timeout automático após inatividade
- **Dados:** Proteção contra SQL Injection (PreparedStatement)
- **Senhas:** Hash com salt usando BCrypt

## 📱 Telas Principais

### **Página de Login**
- Login único para todos os perfis
- Redirecionamento automático conforme perfil
- Recuperação de senha

### **Dashboard do Professor**
- Lista de turmas atribuídas
- Chamadas recentes
- Justificativas pendentes
- Menu rápido para nova chamada

### **Painel do Aluno**
- Status de presença
- Formulário de justificativa
- Avisos e eventos
- Histórico de faltas

### **Área do Setor de Apoio**
- Gerenciador de eventos
- Publicador de avisos
- Validador de justificativas
- Relatórios administrativos

## 🧪 Testes

### **Testes Manuais**
1. Fluxo completo de chamada
2. Justificativa de falta
3. Publicação de evento
4. Geração de relatório

### **Casos de Teste Críticos**
- Login com credenciais inválidas
- Tentativa de acesso não autorizado
- Validação de formulários
- Responsividade em diferentes dispositivos

## 🐛 Solução de Problemas Comuns

### **Problema: Erro de conexão com banco de dados**
```
Solução: Verificar db.properties e status do MySQL
```
---

**Desenvolvido como projeto acadêmico do SENAI**
  
---

📅 **Cronologia do Projeto:**
- **Início do desenvolvimento:** Fevereiro 2025 (1º semestre)
- **Término do desenvolvimento:** Novembro 2025

---
