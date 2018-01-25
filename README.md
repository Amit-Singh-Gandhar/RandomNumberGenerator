                                               Random Number Generation Algorithm(Explanation)

A custom random number generation algorithm which is 73% biased to the higher number.

To generate n = 100 number on a bias of 73% to the higher numbers in the range between a = 1 and b = 10 (both a and b are inclusive), we calculate the value of p and q. p holds the counting of higher numbers and q stores the counting of lower numbers. To find the value of p, we multiply 0.73 with n. For calculating the value of q, we multiply n with the 0.27.  By doing this, we get 73% higher numbers and 27% lower numbers in generated numbers. 
Now we generate random numbers with the help of following formula.
 
num = (num + System time in ticks) mod (b+1)

After generating the value of num, we check whether num is less than the lower bound(a) or not. If the condition is true, we will generate a new number and check the above condition again. If the condition is false, we will check other two conditions which are used to generate favourable numbers as output. According to the first condition, if generated number num is greater than or equal to the median of given range and the value of p is not equal to 0, the generated number num will be printed otherwise we move to the second condition. Same for the second condition, if generated number num is less than to the median of given range and the value of q is not equal to 0, the generated number num will be printed otherwise we move forward.
This loop is continued until the values of both p and q are not equal to the zero. This algorithm generates 73% numbers which are greater than or equal to the median of given range and 27% numbers which are less than to the median of given range.
