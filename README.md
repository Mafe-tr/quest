# quest
Questionario Questão 7


s = input()
count = 0
tamanho = len(s) + 1
indice = int(len(s)/2)
if len(s) % 2 == 0:
    for i in range(0,indice):
        if s[i] != s[-1*(i+1)]:
            count = count + 1
    if count == 1:
        print('ON')
    else:
        print('OFF')
else:
    for i in range(0,len(s)):
        if s[i] != s[-1*(i+1)]:
            count = count + 1
    if count == 0:
        print('ON')
    else:           
        final = int(count/2) 
        if final == 1:
            print('ON')
        else:
            print('OFF')
