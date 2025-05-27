# 💻 Desafio: Configuração de Banco de Dados no Microsoft Azure

Este repositório é resultado de um laboratório prático com o objetivo de **configurar uma instância de banco de dados na plataforma Microsoft Azure**. Ele serve como **material de apoio** com resumos, anotações e dicas úteis para revisões e futuras implementações.

---

## 📚 Resumo

O **Azure SQL Database** é um serviço de banco de dados relacional na nuvem, totalmente gerenciado pela Microsoft. Ele oferece escalabilidade, alta disponibilidade e segurança com mínimo esforço de administração.

---

## 🛠️ Etapas para Configuração da Instância no Azure

1. **Acesse o Portal Azure:**  
   [https://portal.azure.com](https://portal.azure.com)

2. **Crie um Recurso do Tipo “Banco de Dados SQL”**
   - Vá em *Criar um recurso > Bancos de Dados > Banco de Dados SQL*.
   - Dê um nome ao banco e escolha o grupo de recursos (ou crie um novo).

3. **Configure o Servidor**
   - Crie um novo servidor informando:
     - Nome único do servidor.
     - Login de administrador.
     - Senha.
     - Região (ex: "Brazil South").

4. **Defina o Plano de Preços**
   - Escolha a camada de desempenho (Basic, Standard, Premium).
   - Use a opção de "uso gratuito" se estiver disponível.

5. **Regras de Firewall**
   - Adicione seu IP atual para permitir conexões externas.
   - Você pode alterar isso depois em *Segurança > Conexões de Firewall*.

6. **Conecte-se ao Banco de Dados**
   - Use **Azure Data Studio**, **SQL Server Management Studio (SSMS)** ou qualquer cliente compatível com SQL Server.
   - String de conexão está disponível no painel do banco.

---

## 📝 Anotações Importantes

- **Azure cria automaticamente o banco de dados `master`** – não o utilize para aplicações.
- **Evite senhas fracas**: Azure exige critérios fortes para criação de senha.
- **Sempre revise as políticas de firewall** ao usar uma nova rede/IP.
- **Tenha atenção aos custos**, especialmente se sair do plano gratuito.

---

## 💡 Dicas Úteis

- Use o **monitoramento integrado do Azure** para verificar desempenho e auditoria.
- Faça **backups automatizados** com a opção “Geo-redundante” para mais segurança.
- Utilize **tags** para organização e rastreamento de custos em múltiplos recursos.
- Aproveite o **Query Performance Insight** para otimizar consultas SQL.

---

## 📎 Referências

- [Documentação oficial do Azure SQL Database](https://learn.microsoft.com/pt-br/azure/azure-sql/)
- [Azure Data Studio](https://learn.microsoft.com/pt-br/sql/azure-data-studio/)
- [Portal Azure](https://portal.azure.com)

---

## ✅ Status do Desafio

✅ Instância criada  
✅ Conexão testada  
✅ Documentação e dicas registradas  
