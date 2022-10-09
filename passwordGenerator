import random
def calcPassword():
    qtyOfChar = int(input(' - Enter how many characters must the password be:\n'))

    chars = {
    'lowers': 'abcdefghijklmnopqrstuvwxyzç',
    'uppers': 'ABCDEFGHIJKLMNOPQRSTUVWXYZÇ',
    'numbers': '0123456789',
    'specials': '!@#$%¨&*()_+=\/{}:;.,'
    }

    outPass = ''
    outPassLs = []
    charsLeft = qtyOfChar
    while charsLeft > 0:
        seed = random.choice(['lowers','uppers','numbers','specials'])

        n = random.randint(1, charsLeft//5+1)
        charsLeft = charsLeft - n
        outPassLs += random.choices(chars[seed], k = n)
            
    outPass = ''.join(outPassLs)

    print(outPass)

calcPassword()