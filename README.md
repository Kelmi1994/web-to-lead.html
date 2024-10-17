# web-to-lead.html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulário Web-to-Lead</title>
    <style>
        /* Aqui vai o CSS que já foi configurado */
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 20px;
            background-color: #f4f4f4;
        }

        form {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border: 1px solid #ccc;
            width: 100%;
            max-width: 600px;
        }

        form input[type="text"],
        form select,
        form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }

        form input[type="submit"] {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <form action="https://webto.salesforce.com/servlet/servlet.WebToLead?encoding=UTF-8&orgId=00D2E000000pEtk" method="POST">
        <p>*Campos obrigatórios</p>
        <input type="hidden" name="oid" value="00D2E000000pEtk">
        <input type="hidden" name="retURL" value="https://www.exemplo.com/obrigado">

        <label for="first_name">Primeiro Nome</label>
        <input id="first_name" maxlength="40" name="first_name" size="20" type="text" required/><br>

        <label for="last_name">Sobrenome</label>
        <input id="last_name" maxlength="80" name="last_name" size="20" type="text" required/><br>

        <label for="email">Email</label>
        <input id="email" maxlength="80" name="email" size="20" type="text" required/><br>

        <label for="phone">Telefone</label>
        <input id="phone" maxlength="40" name="phone" size="20" type="text" required/><br>

        <label for="company">Empresa</label>
        <input id="company" maxlength="40" name="company" size="20" type="text" required/><br>

        <!-- Outros campos que você adicionou -->
        
        <input type="submit" value="Enviar">
    </form>
</body>
</html>
