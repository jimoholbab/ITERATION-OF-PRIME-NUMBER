from math import sqrt, floor

num = int(input("Enter a number: "))
def Primes(maximum):
    numbers = list(range(2,maximum+1))
    primes = []
    
    while numbers[0] <= floor(sqrt(maximum)):
        x = numbers[0]
        primes.append(x)
        numbers.remove(x)
        for i in numbers:
            if i % x == 0:
                numbers.remove(i)
    return (x)

print(Primes (num))
