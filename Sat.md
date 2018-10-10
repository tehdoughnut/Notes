## Recursion

**Examples in class**

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


## Exercise : power iter

Write an iterative function iterPower(base, exp) that calculates the exponential  by simply using successive multiplication. For example, iterPower(base, exp) should compute  by multiplying base times itself exp times. Write such a function below.

This function should take in two values - base can be a float or an integer; exp will be an integer  0. It should return one numerical value. Your code must be iterative - use of the ** operator is not allowed.

    def iterPower(base, exp):
        '''
        base: int or float.
        exp: int >= 0

        returns: int or float, base^exp
        '''
        result = 1
        for count  in range(exp):
            result = result * base

        return result  
<br/>

    def iterPower2(base, exp):
        '''
        base: int or float.
        exp: int >= 0

        returns: int or float, base^exp
        '''
        result = 1
        while exp > 0:
          result = result * base
          exp = exp -1


        return result




















