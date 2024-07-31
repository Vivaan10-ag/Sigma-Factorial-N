# Sigma-Factorial-N
def factorial(n):
  if n == 0 or n == 1:
    return 1
  else:
    return n*factorial(n-1)
def sum_of_total_factorial_series(x):
  total_sum = 1
  for i in range (1, x + 1):
    total_sum += factorial(i)
  return total_sum
x = int(input("Enter a number to find the factorial of: "))
y = str(input("Enter a number to find the sum (yes/no): "))
if y.lower() == "Yes":
  print("The sum of factorials till", x, "is", sum_of_total_factorial_series(x))
  fact = 1
  if x < 0:
    print("The factorial for negative numbers does not exist")
  elif x == 0:
    print("The factorial of 0 is 1")
  else:
    for i in range (1, x + 1):
      fact = fact * i
    print ("The factorial of ", x, "is", fact)
else:
  fact = 1
  if x < 0:
    print ("The factorial for negative number does not exist)\
  elif x == 0:
      print ("The factorial of 0 is 1")\
  else:
    for i in range (1, x + 1):
      fact = fact * i
    print ("The factorial of ", x, "is", fact)
    
