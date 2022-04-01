# CALCULADORA-DE-COMBUSTIVEL-PARA-PREVER-GASTOS-EM-VEICULOS-FLEX-Gasolina-e-Álcool

print('\n\n===============================================================================')
print('===============================================================================')
print('''CALCULADORA DE COMBUSTÍVEL
PARA PREVER GASTOS EM VEÍCULOS FLEX POR QUILÔMETROS RODADOS (Gasolina e Álcool)''')
print('===============================================================================')
print('===============================================================================')

precoEtanol = float(input('Qual é o preço do litro de etanol? \nR$'))
precoGasolina = float(input('Qual é o preço do litro de gasolina? \nR$'))

kmPorLitrodeEtanol = float(input('Quantos quilômetos faz seu carro com 1 litro de etanol? \nKm:'))
kmPorLitrodeGasolina = float(input('Quantos quilômetos faz seu carro com 1 litro de gasolina? \nKm:'))

kmPercorrer = float(input('Quantos quilômetros você vai percorrer nessa sua viagem? '))

#ETANOL
titulo1 = 'ETANOL'
print(f'\n\n\n{titulo1:=^36}')
litrosDeEtanolNecessarios = kmPercorrer/kmPorLitrodeEtanol
valorGastoComLitrosDeEtanol = litrosDeEtanolNecessarios*precoEtanol
print(f'\n{litrosDeEtanolNecessarios:.2f} litros\né a quantidade de etanol necessária para percorrer essa distância.')
print(f'\nR${valorGastoComLitrosDeEtanol:.2f}\né o valor a ser pago por essa quantidade de etanol.')


#GASOLINA
titulo1 = 'GASOLINA'
print(f'\n\n\n{titulo1:=^36}')
litrosDeGasolinaNecessarios = kmPercorrer/kmPorLitrodeGasolina
valorGastoComLitrosDeGasolina = litrosDeGasolinaNecessarios*precoGasolina
print(f'\n{litrosDeGasolinaNecessarios:.2f} litros\né a quantidade de gasolina necessária para percorrer essa distância.')
print(f'\nR${valorGastoComLitrosDeGasolina:.2f}\né o valor a ser pago por essa quantidade de gasolina.')

print('===============================================================================')
print('===============================================================================')
