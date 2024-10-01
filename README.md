# Tutorial: Como Criar uma Conta Estudantil no Azure, Configurar Azure SQL Server e Usar DBeaver para Conexão

Neste tutorial, você aprenderá a configurar uma conta gratuita no Azure para estudantes, criar um banco de dados no Azure SQL Server, e usar o DBeaver como cliente de SQL para gerenciar seu banco de dados.

## Parte 1: Criando uma Conta Estudantil no Azure

* Passo 1: Acessar a página de inscrição do Azure para estudantes*

1. Acesse o link: [Azure para Estudantes](https://azure.microsoft.com/pt-br/free/students).
2. Clique no botão **Iniciar gratuitamente**.

* Passo 2: Fazer login ou criar uma conta Microsoft

1. Se você já possui uma conta Microsoft (Hotmail, Outlook, etc.), faça login.
2. Caso contrário, crie uma nova conta.

* Passo 3: Verificação de estudante

1. A plataforma solicitará uma verificação de sua condição de estudante. Será necessário fornecer um endereço de e-mail institucional (ex.: <seunome@universidade.edu.br>).
2. Após a verificação, você terá acesso a serviços gratuitos no Azure, incluindo créditos de até **US$ 100** sem necessidade de cartão de crédito.

---

## Parte 2: Criando um Grupo de Recursos e Configurando o Banco de Dados Azure SQL Server

* Passo 1: Criando um Grupo de Recursos

1. Acesse o portal do Azure: [Azure Portal](https://portal.azure.com/).
2. No menu à esquerda, clique em **Grupos de recursos**.
3. Clique em **Adicionar** para criar um novo grupo de recursos.
   * **Nome**: Escolha um nome para o grupo de recursos (ex.: `grupo-estudo`).
   * **Região**: Selecione uma região que melhor atenda às suas necessidades (ex.: `Brasil Sul`).
4. Clique em **Revisar + Criar** e em seguida **Criar**.

* Passo 2: Criando o Banco de Dados Azure SQL Server

1. No portal do Azure, no menu à esquerda, clique em **Criar um recurso**.
2. Na barra de pesquisa, digite **SQL Database** e selecione a opção correspondente.
3. Clique em **Criar**.

    **Configurações do Banco de Dados:**

    * **Assinatura**: Selecione sua assinatura gratuita de estudante.
    * **Grupo de Recursos**: Selecione o grupo de recursos que você criou no passo anterior (`grupo-estudo`).
    * **Nome do Banco de Dados**: Escolha um nome (ex.: `banco-estudante`).
    * **Servidor**: Clique em **Criar novo** e configure seu servidor SQL.
    * **Nome do Servidor**: Escolha um nome exclusivo (ex.: `servidor-estudante`).
    * **Localização**: Escolha a mesma localização usada para o grupo de recursos.
    * **Autenticação**: Configure um login e senha para o administrador do SQL Server. **Guarde essa informação**.

4. Após configurar, clique em **Revisar + Criar** e, em seguida, **Criar**.

---

### Parte 3: Baixando e Configurando o DBeaver

* Passo 1: Baixando o DBeaver

1. Acesse o site oficial do DBeaver: [DBeaver.io](https://dbeaver.io/).
2. Clique em **Download** e escolha a versão apropriada para o seu sistema operacional (Windows, macOS ou Linux).
3. Siga as instruções de instalação.

* Passo 2: Conectando-se ao Azure SQL Server com o DBeaver

1. Abra o DBeaver após a instalação.
2. No menu superior, clique em **File** e depois em **New** para adicionar uma nova conexão.
3. Selecione **SQL Server** e clique em **Next**.
4. Preencha os seguintes dados:
   * **Host**: O endereço do seu servidor SQL criado no Azure (ex.: `servidor-estudante.database.windows.net`).
   * **Database**: O nome do banco de dados (ex.: `banco-estudante`).
   * **Username**: Seu login de administrador SQL configurado durante a criação do banco de dados.
   * **Password**: A senha definida para o administrador.

5. Clique em **Test Connection** para verificar a conexão. Se tudo estiver correto, a conexão será estabelecida.
6. Clique em **Finish** para salvar a configuração.

Agora você pode gerenciar seu banco de dados no Azure SQL Server diretamente pelo DBeaver!

---

### Conclusão

Você configurou com sucesso uma conta no Azure, criou um grupo de recursos, implementou um banco de dados no Azure SQL Server e conectou-se a ele usando o DBeaver. Esse ambiente permite que você experimente o uso de bancos de dados na nuvem com uma interface gráfica poderosa para administrar suas tabelas e consultas.

Se tiver dúvidas ou precisar de mais recursos, não hesite em consultar a [documentação oficial do Azure](https://docs.microsoft.com/pt-br/azure/) e do [DBeaver](https://dbeaver.io/documentation/).
