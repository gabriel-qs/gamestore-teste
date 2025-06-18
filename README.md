# gamestore-teste

A aplicação utiliza **testes unitários** e **de integração** para garantir a robustez das operações de CRUD relacionadas a produtos.  

#### **Tecnologias e Ferramentas**  
✅ **Jest** – Framework de testes para execução e avaliação.  
✅ **Prisma Client** – ORM para interações com o banco de dados (mockado em testes).  
✅ **ts-jest** – Suporte a TypeScript nos testes.  
✅ **Mocks** – Simulação de chamadas ao banco de dados para isolamento dos testes.  

---

### **Testes Unitários** 🔍  
- **Foco**: Validar a lógica individual das funções na camada de ações (`src/actions/products`).  
- **Abordagem**:  
  - Mocking do **Prisma Client** para evitar dependência de um banco de dados real.  
  - Cobertura de cenários de **sucesso** e **falha**.  
  - Testes **isolados**, **rápidos** e **determinísticos**.  

---

### **Testes de Integração** 🔗  
- **Foco**: Validar a interação entre a camada de ações e o banco de dados simulado.  
- **Testes Implementados**:  
  - **`create-product.test.ts`** → Criação de produtos.  
  - **`get-products.test.ts`** → Leitura de produtos.  
  - **`update-product.test.ts`** → Atualização de produtos.  
  - **`delete-product.test.ts`** → Exclusão de produtos.  

---

### **Configuração do Ambiente** ⚙️  
- **Ambiente local** sem dependência de serviços externos.  
- **Mocks manuais** das interações com o Prisma para segurança nos testes.  
- **Suporte a TypeScript** via `ts-jest`.  

---

### **Resultados Esperados** 🎯  
- **Cobertura completa** das operações CRUD.  
- **Comportamento consistente** em diferentes cenários.  
- **Feedback rápido** durante o desenvolvimento.  

