***A palindromic number reads the same both ways. The largest palindrome made from the product of two 2-digit numbers is 9009 = 91 × 99.
Find the largest palindrome made from the product of two 3-digit numbers.***

```r
{
  n = as.integer(readline(prompt = "Enter a number :"))
  
  rev = 0
  num = n
  
  while (n > 0) {
    r = n %% 10
    rev = rev * 10 + r
    n = n %/% 10
  }
  
  if (rev == num)
  {
    print(paste("Number is palindrome :", rev))
  }
  else{
    print(paste("Number is not palindrome :", rev))
  }
}
```
