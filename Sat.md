# Recursion

<b>Examples in class</b>

    def multiter(a,b):
      result = 0
      print("at the beginning, result is",result,"and a is",a,"and b is",b)
      while b > 0:
        result = a + result
        b = b - 1
        print("at the end of the loop, result is",result,"and a is",a,"and b is",b)
      return result
<break></break>

    def multiter2(a,b):
      result = 0
      print("at the beginning, result is",result,"and a is",a,"and b is",b)
      for count in range(b):
        result = result + a
        print("at the end of the loop, count is",count,"and result is",result,"and a is",a,"and b is",b)
      return result
<break></break>

    def recurmult(a,b):
      if b == 1:
        return a
      else:
        return a + recurmult(a, (b-1))
<break></break>

    def fact(n):
      if n == 1:
        return 1
      else:
        return n * fact(n-1)





























