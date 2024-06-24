# Convertidor-de-Euros-a-Dolar
Programa de conversión de Euros a Dólar

Backend

############### PROGRAMA DE CONVERSION DE EUROS A DOLLAR ###############

# Desarrollo de la funcion convertidor.
def convertidor():
    # Define la tasa de conversion.
    tasa_conversion = 1.07
    # Solicita al usuario que ingrese la cantidad en euros.
    euros = input("ingrese la cantidad en euros: ")
    
    # Convierte la entrada a un numero flotante.
    try:
        euros = float(euros)
    except ValueError:
        print("Por favor, ingrese un número válido.")
        return
    
    # Realiza la conversión
    dolares = euros * tasa_conversion
    
    # Muestra el resultado
    print(f"{euros} Euros son equivalentes a {dolares} Dólares.")
    
def espacio():
    print("***************************************************")
       
    
def main():
    while True:
        convertidor()
        espacio()
        respuesta = input("¿Desea realizar otra conversión? (s/n): ")
        if respuesta.lower() == 'n':
            break
        elif respuesta.lower() == 's':
            continue
        else:
            print("Respuesta no válida. Intente nuevamente.")

if __name__ == "__main__":
    main()
