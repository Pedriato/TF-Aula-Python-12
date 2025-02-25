#Inventário de Produtos

nome = ()
preço = ()
quantidade = ()
produtos = ()

def mostrar_menu():
    print("Escolha uma opção:")
    print("1. Adicionar")
    print("2. Remover")
    print("3. Listar os Produtos")
    print("4. Sair")

def obter_escolha():
    escolha = input("Digite o número da sua escolha: ")
    return escolha

def main():
    while True:
        mostrar_menu()
        escolha = obter_escolha()

        if escolha == "1":
            def solicitar_dados_usuario():
                nome = input("Nome do Produto: ")
                preço = input("Preço do Produto: ")
                quantidade = input("Quantidade desejada: ")
                print ("Produto adicionado com sucesso!")
        elif escolha == "2":
            

            print("Você escolheu a Opção 2.")
        elif escolha == "3":
            produtos = {
            "Nome": nome,
            "Preço": preço,
            "Quantidade": quantidade
}
            print(nome, preço, quantidade)
        elif escolha == "4":
            print("Saindo...")
            break
        else:
            print("Escolha inválida. Tente novamente.")

if __name__ == "__main__":
    main()

