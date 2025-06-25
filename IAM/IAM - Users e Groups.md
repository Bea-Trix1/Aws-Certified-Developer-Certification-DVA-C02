# IAM - Identidade e Gerenciamento de Acesso

- **Serviço global**
    - Usado ao criar a conta **Root**  
        - **Não** deve ser utilizada para outras tarefas, nem compartilhada

-    ## Usuários e Grupos

     **Usuários**: Pessoas dentro da organização, agrupadas por responsabilidade
     **Grupos**: Devem conter **apenas usuários** (não outros grupos)
     Nem todo usuário precisa pertencer a um grupo  
        - *Não é recomendável, mas é possível*
     Usuários podem participar de **mais de um grupo**



 ## Por que precisamos do IAM?

- **Permissões**: Permitem a um usuário ou grupo alterar políticas

        - Exemplo: Escrever em uma instância EC2
        - Exemplo: Listar bancos de dados
- **Políticas**: Definem as permissões dos usuários
  
        - Princípio de confiança **zero**
        - Princípio do **menor privilégio**

    ---

    > **Atenção:**  
    > Contas **Root** não devem ser usadas no dia a dia.  
    > Utilize apenas para criar usuários administradores, grupos ou outros usuários dentro da organização.