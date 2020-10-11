import math

ITERATIONS = 20

def my_cos(x):
    """
    Вычисление коминуса при помощи частичного суммирования
    ряда Тейлора для окрестности 0, что верно только для маллых углах
    """
    x_pow = 1 
    multiplier = 1
    partial_sum = 1
    for n in range(1, ITERATIONS):
        x_pow *= x**2  # Каждый слеющий член больше в X^2 Раз + остальное учтено далее
        multiplier *= -1 / (2*n-1) / (2*n )  # (-1)^n и факториал
        partial_sum += x_pow * multiplier
    
    return partial_sum

print(help(math.cos), math.cos(2))
print(help(my_cos), my_cos(2))
