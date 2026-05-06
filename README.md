# 📚 Estudo de Banco de Dados

Repositório dedicado ao aprendizado e prática de conceitos fundamentais em **Bancos de Dados** e **SQL**.

## 📋 Conteúdo do Repositório

### 📁 Arquivos Principais

| Arquivo | Descrição |
|---------|-----------|
| **CriandoBanco.sql** | Scripts SQL prático com exemplos de criação de tabelas, inserção de dados, alterações estruturais e joins |
| **CodigosDB.txt** | Referência completa de comandos SQL básicos e operações comuns |
| **Queries.txt** | Exemplos de queries prontas para execução |

## 🎯 Tópicos Abordados

### ✅ Conceitos Básicos
- Criação e exclusão de bancos de dados
- Criação e manipulação de tabelas
- Tipos de dados e restrições (PRIMARY KEY, FOREIGN KEY, UNIQUE, NOT NULL)

### ✅ Operações CRUD
- **CREATE**: Inserção de dados com `INSERT INTO`
- **READ**: Consultas com `SELECT` e filtros
- **UPDATE**: Atualização de registros
- **DELETE**: Remoção de dados

### ✅ Operações Avançadas
- **ALTER TABLE**: Modificação de estrutura de tabelas
- **INNER JOIN**: Junção de múltiplas tabelas
- **Normalização**: Estruturação de tabelas relacionadas com Foreign Keys
- **Filtros**: WHERE, BETWEEN, IN, NOT IN, LIKE
- **Ordenação**: ORDER BY (ASC/DESC)
- **Agregação**: COUNT, LIMIT, OFFSET

## 🚀 Como Usar

1. **Abra um cliente SQL** (MySQL, MariaDB, etc.)
2. **Execute os scripts** na sequência desejada
3. **Estude os exemplos** em `CodigosDB.txt` para entender cada comando
4. **Adapte as queries** para seus próprios projetos

### Exemplo de Execução

```sql
-- Selecionar o banco de dados
USE banco_donkey;

-- Criar tabela
CREATE TABLE conta (
    id INT NOT NULL AUTO_INCREMENT,
    numero INT(4) NOT NULL,
    agencia INT(8) NOT NULL,
    tp_conta VARCHAR(10) NOT NULL DEFAULT 'Corrente',
    cliente VARCHAR(100) NOT NULL,
    saldo DECIMAL(13, 2) NOT NULL,
    PRIMARY KEY (id)
);

-- Inserir dados
INSERT INTO conta (numero, agencia, cliente, saldo) 
VALUES (1001, 12345678, 'Abner Amos', 1000);

-- Consultar dados
SELECT * FROM conta WHERE saldo > 1000;
```

## 📖 Estrutura de Aprendizado

O repositório segue uma progressão de complexidade:
1. **Fundamentos**: Criação de banco e tabelas
2. **Manipulação básica**: INSERT, SELECT, UPDATE, DELETE
3. **Estrutura avançada**: ALTER TABLE, constraints
4. **Relacionamentos**: Foreign Keys e INNER JOINs
5. **Queries complexas**: Múltiplas condições e joins

## 🛠️ Tecnologias

- **SQL**: Linguagem de consulta
- **Banco de Dados**: MySQL/MariaDB (compatível com outros RDBMS)

## 📝 Notas Importantes

- Os scripts incluem comentários em português para melhor compreensão
- Utilize aliases para melhorar a legibilidade das queries
- Sempre teste em um banco de dados de desenvolvimento antes de usar em produção
- A normalização de tabelas é fundamental para manter a integridade dos dados

## 🤝 Contribuindo

Sinta-se livre para:
- Adicionar novos exemplos
- Melhorar a documentação
- Sugerir correções ou otimizações
- Compartilhar casos de uso reais

## 📞 Contato

Desenvolvido por **Abner Amos**

---

**Última atualização**: 2026-05-06
