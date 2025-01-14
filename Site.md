# **Construindo um site**

Devido ao avanço da tecnologia, não é possível criar um clone de http://www.facebook.com. Tal link é automaticamente redirecionado
ao site com https, que impede a transmissão direta de dados e possui defesas e criptografia.

Desse modo, o codigo a seguir foi usado para criar um localhost simples e copia-lo usando o setoolkit no Kali Linux.

## **Códigos**

* Criando arquivo html:                                                                                                                                             
&nbsp;&nbsp;nano index.html
* Formulário simples de login:
    ```
    <!DOCTYPE html>
    <html>
    <head>
        <title>Formulário de Login</title>
    </head>
    <body>
        <h2>Login</h2>
        <form action="http://localhost:8080" method="POST">
            Usuário: <input type="text" name="usuario"><br>
            Senha: <input type="password" name="senha"><br>
            <input type="submit" value="Entrar">
        </form>
    </body>
    </html>
* Iniciando o servidor:
&nbsp;&nbsp;python3 -m http.server 'porta' (Nesse projeto foi utilizado a porta 8080)


#### **OBS:**
&nbsp;&nbsp;O código do servidor deve ser escrito em um diretório diferente do setoolkit.

