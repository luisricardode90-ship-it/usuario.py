usuario = "admin"
senha = "123"

cadastro = "sim"

while cadastro == "sim":

    print("#####################################################################################################")
    print("                 SISTEMA DE CADASTRO DE USUÁRIOS")
    print("#####################################################################################################")

    usuario_digitado = input("Login: ")
    senha_digitada = input("Senha: ")

    if usuario_digitado == usuario and senha_digitada == senha:

        print("Login realizado com sucesso!")
    else:

        menu = 0

        while menu != 6:

            print("""
================ MENU PRINCIPAL ================

[1] Inserir usuário
[2] Pesquisar usuário
[3] Remover usuário
[4] Lista de todos os usuários
[5] Logout
[6] Encerrar

=================================================
""")

            opcao = input("Digite a opção desejada: ")

            if opcao == "5":
                print("Logout realizado!")
                break

            elif opcao == "6":
                print("Programa encerrado!")
                cadastro = "não"
                menu = 6

        else:
            print("Usuário ou senha incorretos!")
