SLE
*Ver o usuário atual:
    
    ```
    SELECT user();
    ```
    
- **Ver a versão exata do banco:**
    
    SQL
    
    ```
    SELECT version();
    ```
    

### **2. Mapeando os Bancos de Dados**

O servidor MariaDB é como um armário gigante que guarda várias gavetas (os bancos de dados). Primeiro, precisamos ver quais gavetas existem.

- **Listar todos os bancos de dados:**
    
    SQL
    
    ```
    SHOW DATABASES;
    ```
    
- **Acessar um banco de dados específico:** Quando você encontrar um nome interessante (fuja dos padrões como `information_schema` ou `performance_schema` por enquanto; procure por coisas como `wordpress`, `app_db`, `users`, etc.), você precisa "entrar" nele:
    
    SQL
    
    ```
    USE nome_do_banco;
    ```
    
    _(Você verá o prompt mudar de `[(none)]` para `[nome_do_banco]`)_
    

### **3. Inspecionando as Tabelas**

Dentro do banco de dados (a gaveta), existem várias pastas (as tabelas).

- **Listar todas as tabelas do banco atual:**
    
    SQL
    
    ```
    SHOW TABLES;
    ```
    
- **Ver a estrutura de uma tabela:** Antes de extrair os dados, é útil saber quais colunas aquela tabela tem (ex: `id`, `username`, `password`, `email`).
    
    SQL
    
    ```
    DESCRIBE nome_da_tabela;
    ```
    

### **4. Extraindo o "Ouro" (Os Dados)**

Esta é a parte onde você encontra as informações que precisa.

- **Ver TUDO dentro de uma tabela:** Isso despeja todo o conteúdo da tabela na sua tela. Em ambientes reais pode travar o terminal se a tabela for gigante, mas em CTFs costuma ser seguro.
    
    SQL
    
    ```
    SELECT * FROM nome_da_tabela;
    ```
    
- **Ver apenas colunas específicas:** Se a tabela tiver muita poluição visual, você pode filtrar apenas o que importa (por exemplo, se o `DESCRIBE` te mostrou que existem colunas chamadas `user` e `pass`):
    
    SQL
    
    ```
    SELECT user, pass FROM nome_da_tabela;
    ```