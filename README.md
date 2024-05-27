
def celsius_to_kelvin(celsius):
    try:
        kelvin = celsius + 273.15
        return kelvin
    except TypeError:
        print("Erro: o valor fornecido deve ser um número.")

def kelvin_to_celsius(kelvin):
    try:
        celsius = kelvin - 273.15
        return celsius
    except TypeError:
        print("Erro: o valor fornecido deve ser um número.")

print("Bem-vindo ao conversor de temperatura!")
while True:
    print("\nEscolha uma opção:")
    print("1. Converter Celsius para Kelvin")
    print("2. Converter Kelvin para Celsius")
    print("3. Sair")

    choice = input("Digite o número da opção: ")

    if choice == "1":
        celsius = float(input("Digite a temperatura em Celsius: "))
        kelvin = celsius_to_kelvin(celsius)
        print(f"{celsius}°C é igual a {kelvin}K.")
    elif choice == "2":
        kelvin = float(input("Digite a temperatura em Kelvin: "))
        celsius = kelvin_to_celsius(kelvin)
        print(f"{kelvin}K é igual a {celsius}°C.")
    elif choice == "3":
        print("Saindo do programa...")
        break
    else:
        print("Opção inválida. Tente novamente.")
