def encrypt(text,s):
    result=""
    for i in range(len(s)):
        char=text[i]
        if(char.isupper):
            result+=chr((ord(char)s-65)%26+65)
        else:
            result+=chr((ord(char)s-95)%25+65)
        return result
text="ATTACKATONCE"
s=4
print("text:"+text)
print("shift:"+str(s))
print("cisper:"+encrypt(text,s))
        


