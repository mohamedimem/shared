### string formating

```python
print("hello %4s"%'world') # hello world
# %4s means the string must be 4 characters at least if not it adds spaces in the start
# here 5 chars it added nothing
print("hello %6s"%'world') # hello  world (added one space)
print("hello %6s %4s"%('world','man')) # hellow  world  man
# %d number %f floating point number
print("%s number is :%f"%('my',5)) # my number is : 5.000000 (%f is %.6f by default)
print("%s number is :%.10f"%('my',5)) # my number is : 5.0000000000
print("%s number is :%6.2f"%('my',5)) # my number is :  5.00 (will add two more space cuz len('  5.00')=6)
print("%s number is :%9f"%('my',5)) # my number is : 5.000000 (added one space len(' 5.000000')=9)
print("%5.6o"%(25)) # its octal of 25 (31)
# 6 here the size of the output it adds zeros in the start
# 5 is the size too but without adding zeros
=> # 000031 (adding zeros to get the size to 6 override 5 )
print("%6.5o"%(25)) #  00031 (adding zeros with 1 empty space )
print("%E"%(1.2547)) # E exponential notation default %.6E (1.254700+E04) (6 number of decimals)
print("%.2E"%(1.2547)) # 1.25+E00
print("%9.2E"%(1.2557)) #  1.26E+00 (add one space)
print("%6.0E"%(125575.48)) # 1E+05 (adds one space)
print("%.15E"%(0.0000000000000000000012557548))
#1.255754800000000E-21(21 number of zeros 0.00....)
```
