def calcular_billetes(monto):
    print("\nMonto: $" + str(monto))

    billetes_500 = monto // 500
    monto = monto - (billetes_500 * 500)

    billetes_200 = monto // 200
    monto = monto - (billetes_200 * 200)

    billetes_100 = monto // 100
    monto = monto - (billetes_100 * 100)

    billetes_50 = monto // 50
    monto = monto - (billetes_50 * 50)

    total = billetes_500 + billetes_200 + billetes_100 + billetes_50

    print("Billetes de $500:", billetes_500)
    print("Billetes de $200:", billetes_200)
    print("Billetes de $100:", billetes_100)
    print("Billetes de $50: ", billetes_50)
    print("Total de billetes:", total)


# PRUEBAS
calcular_billetes(1850)
calcular_billetes(700)
calcular_billetes(50)
