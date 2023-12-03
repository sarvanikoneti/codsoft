# codsoft
import random
import string
#defining the random password generator function with length(l)
def rgp(l):
#taking all possible characters that can be used to generate password
  c=string.ascii_letters+string.digits+string.punctuation
#generating password of desired length
  P=''.join(random.choice(c) for i in range(l))
  return P
#taking input from the user for length of password
pl=int(input("Enter the length of password:"))
password=rgp(pl)
#printing the generated password on screen
print(f"Generated password is:{password}")
       
