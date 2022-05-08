# redo_topic_currency
list_A_dolar = []
list_A_euro = []
list_A_ndt = []

list_B_dolar = []
list_B_euro = []
list_B_ndt = []

list_C_dolar = []
list_C_euro = []
list_C_ndt = []

def doitiendolar(name, quant):
    sotien = round(quant / 23000, 2)
    i = str(sotien) + str('$')
    if name == 'A':
        list_A_dolar.append(i)
        print(list_A_dolar)
    if name == 'B':
        list_B_dolar.append(i)
        print(list_B_dolar)
    if name == 'C':
        list_C_dolar.append(i)
        print(list_C_dolar)

def doitieneuro(name, quant):
    sotien = round(quant / 24000, 2)
    i = str(sotien) + str('€')
    if name == 'A':
        list_A_euro.append(i)
        print(list_A_euro)
    if name == 'B':
        list_B_euro.append(i)
        print(list_B_euro)
    if name == 'C':
        list_C_euro.append(i)
        print(list_C_euro)

def doitienndt(name, quant):
    sotien = round(quant / 800, 2)
    i = str(sotien) + str('¥')
    if name == 'A':
        list_A_ndt.append(i)
        print(list_A_ndt)
    if name == 'B':
        list_B_ndt.append(i)
        print(list_B_ndt)
    if name == 'C':
        list_C_ndt.append(i)
        print(list_C_ndt)


print('-----bai nay gioi han moi nguoi 2 luot doi tien------')
while True:
    name = input('ten ban la: ')
    if name == 'A':
        if ((len(list_A_dolar) + len(list_A_euro) + len(list_A_ndt)) < 2):

                currency = int(input('loai tien ban muon doi( 1:VND-dolar, 2:VND-euro, 3:VND-ndt): '))
                if currency == 1:
                    quant = int(input('so tien ban muon doi:'))
                    doitiendolar('A', quant)

                if currency == 2:
                    quant = int(input('so tien ban muon doi:'))
                    doitieneuro('A', quant)
                if currency == 3:
                    quant = int(input('so tien ban muon doi:'))
                    doitienndt('A', quant)
        else:
            print('ban het luot doi tien!')

    if name == 'B':
        if ((len(list_B_dolar) + len(list_B_euro) + len(list_B_ndt)) < 2):

                currency = int(input('loai tien ban muon doi( 1:VND-dolar, 2:VND-euro, 3:VND-ndt): '))
                if currency == 1:
                    quant = int(input('so tien ban muon doi:'))
                    doitiendolar('B', quant)

                if currency == 2:
                    quant = int(input('so tien ban muon doi:'))
                    doitieneuro('B', quant)
                if currency == 3:
                    quant = int(input('so tien ban muon doi:'))
                    doitienndt('B', quant)
        else:
            print('ban het luot doi tien!')

    if name == 'C':
        if ((len(list_C_dolar) + len(list_C_euro) + len(list_C_ndt)) < 2):

                currency = int(input('loai tien ban muon doi( 1:VND-dolar, 2:VND-euro, 3:VND-ndt): '))
                if currency == 1:
                    quant = int(input('so tien ban muon doi:'))
                    doitiendolar('C', quant)

                if currency == 2:
                    quant = int(input('so tien ban muon doi:'))
                    doitieneuro('C', quant)
                if currency == 3:
                    quant = int(input('so tien ban muon doi:'))
                    doitienndt('C', quant)
        else:
            print('ban het luot doi tien!')

    if(((len(list_A_dolar) + len(list_A_euro) + len(list_A_ndt)) +(len(list_B_dolar) + len(list_B_euro) + len(list_B_ndt))+
    (len(list_C_dolar) + len(list_C_euro) + len(list_C_ndt)))>=6):
        break
print('-------------------')
print(list_A_dolar)
print(list_A_euro)
print(list_A_ndt)
print(list_B_dolar)
print(list_B_euro)
print(list_B_ndt)
print(list_C_dolar)
print(list_C_euro)
print(list_C_ndt)




