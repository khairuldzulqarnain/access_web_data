# access_web_data
# In this assignment you will read through and parse a file with text and numbers. You will extract all the numbers in the file and compute the sum of the numbers.
# I am using sublime text to saved the text given. The file was rename to as assigmentextractingdata.txt(name may vary depend on You)

import re

hand = open("assigmentextractingdata.txt")
x=list()
for line in hand:
	y = re.findall('[0-9]+',line)
	x = x+y

sum=0
for z in x:
	sum=sum + int(z)

print(sum)

# Execute above code by saved assigemnt.py
# open command prompt and executed the assigment.py
# sum of the number 454046
# Text link is below
# http://py4e-data.dr-chuck.net/regex_sum_1597190.txt
