- [ ] Criar commits pequenos e descritivos  
- [ ] Adicionar instruções básicas de execução no README  

---

### 🔹 2. Configuração do Frontend (Angular)
- [ ] Criar novo projeto Angular → `ng new frontend`
- [ ] Configurar **rotas principais**:
- [ ] `/produtos`
- [ ] `/notas`
- [ ] Criar componentes iniciais:
- [ ] `app-header` (barra de navegação)
- [ ] `cadastro-produtos`
- [ ] `cadastro-notas`
- [ ] `impressao-notas`
- [ ] Criar serviços Angular:
- [ ] `produto.service.ts`
- [ ] `nota.service.ts`
- [ ] Configurar **environments** (`environment.ts`) com URLs das APIs
- [ ] Escolher biblioteca visual (ex: Angular Material, PrimeNG ou Bootstrap)
- [ ] Testar comunicação com backend via HTTPClient + RxJS

---

### 🔹 3. Configuração do Backend (C#)
#### 🟦 Projeto principal
- [ ] Criar solução `.sln` na pasta `/backend`
- [ ] Adicionar dois projetos API:
- [ ] `EstoqueService`
- [ ] `FaturamentoService`
- [ ] Configurar o **Entity Framework Core**
- [ ] Configurar **CORS** para permitir acesso do Angular
- [ ] Adicionar **Swagger** para documentação dos endpoints

#### 🧩 Serviço: EstoqueService
- [ ] Criar modelos:
- [ ] `Produto` → (Id, Codigo, Descricao, Saldo)
- [ ] Criar contexto de banco (`EstoqueContext`)
- [ ] Criar controladores REST:
- [ ] `GET /api/produtos`
- [ ] `POST /api/produtos`
- [ ] `PUT /api/produtos/{id}`
- [ ] Implementar tratamento de exceções globais
- [ ] Testar persistência (SQLite, SQL Server ou outro)

#### 🧾 Serviço: FaturamentoService
- [ ] Criar modelos:
- [ ] `NotaFiscal` → (Id, Numero, Status)
- [ ] `ItemNota` → (ProdutoId, Quantidade)
- [ ] Criar contexto de banco (`FaturamentoContext`)
- [ ] Criar controladores REST:
- [ ] `GET /api/notas`
- [ ] `POST /api/notas`
- [ ] `PUT /api/notas/{id}`
- [ ] Implementar integração com EstoqueService via HTTPClient
- [ ] Tratar exceções e falhas de comunicação
- [ ] Utilizar **LINQ** para consultas e atualizações

---

### 🔹 4. Integração Angular ↔ Backend
- [ ] Configurar URLs dos serviços no frontend (`environment.ts`)
- [ ] Testar chamadas HTTP entre Angular e APIs C#
- [ ] Validar fluxo completo:
- [ ] Cadastro de produto → aparece no backend
- [ ] Criação de nota → comunicação entre serviços
- [ ] Impressão → atualização de status e saldo

---

### 🔹 5. Preparação para próximas etapas
- [ ] Verificar logs e erros globais
- [ ] Criar script ou instrução para rodar ambos os serviços juntos
- [ ] Documentar no README:
- [ ] Como rodar o frontend
- [ ] Como rodar os serviços backend
- [ ] Tecnologias utilizadas
- [ ] Estrutura da solução

---

✅ **Meta da Etapa 1:** Ambiente Angular + C# estruturado, microsserviços criados e comunicação entre eles funcional.
