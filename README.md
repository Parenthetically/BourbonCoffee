BourbonCoffee
=============

Emily's code that Jay typed out

import string

prompt="What phrase do you think might be a palindrome?"
input=raw_input(prompt)
prompt_without_spaces=input.replace(" ","")
print prompt_without_spaces
clean_out_punctuation=prompt_without_spaces.translate(string.maketrans("",""), string.punctuation)
print clean_out_punctuation
clean_out_uppercase=str.lower(clean_out_punctuation)
palindrome=clean_out_uppercase[::-1]
print palindrome
if clean_out_uppercase==palindrome:
    print "Way to go, ace, you found a palindrome somewhere on the internet."
else:
    print "No palindrome here, you derpy f'er."
    
