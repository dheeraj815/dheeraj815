ef is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True

n = int(input("Enter a number: "))
print(is_prime(n))
#task 2
start = int(input("Enter the starting value of the range: "))
end = int(input("Enter the ending value of the range: "))
print(f"Prime numbers between {start} and {end} are:")
for num in range(start, end + 1):
  if is_prime(num):
    print(num, end=" ")
print()
