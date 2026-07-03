import random
letter: str = ("a,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t,u,v,w,x,y,z")
number = ("0,1,2,3,4,5,6,7,8,9,10")
symbol = ("!", "#", "$", "%", "&", "(", ")", "*", "+", ",", "-", ".", "/", ":", ";", "<", "=", ">", "?", "@", "[,],^,_,{,|,},~,")
Linux_syntax = ("sudo-apt-remove","sudo-dnf-remove","reboot","poweroff","sudo-fdisk-l","du","tree","mount-and-umount","tar-cf-my_dir.tar-my_dir","tar-cfz-my_dir.tar-my_tar","tar-xf-my_dir.tar","tar-xfz_my_dir.tar.gz","ls","ls -l","ls -a","pwd","cd","file","mkdir","touch","cat_>_file","cat_file","grep","nano_file","rm--r","mv","cp","rsync","locate","find","whoami","sudo","sudo-apt-install","sudo-dnf-install")
print('**********!!PLEASE TYPE A NUMBER IN A RANGE 1 TO 6 ONLY AND NO MORE FOR ALL CHOICES!!**********')
nr_letters = int(input("How many letters would you like in your password?\n"))
nr_symbols = int(input(f"How many symbols would you like?\n"))
nr_numbers = int(input(f"How many numbers would you like?\n"))
nr_linux_syntax = int(input(f"How many linux syntax would you like?\n"))
random_letters: list[str] = random.sample(letter, nr_letters)
random_numbers = random.sample(number, nr_numbers)
random_symbols = random.sample(symbol, nr_symbols)
random_letters = random.sample(Linux_syntax, nr_linux_syntax)
password = random_letters + random_numbers + random_symbols + random.sample(Linux_syntax, nr_linux_syntax)
random.shuffle(password)
print("PASSWORD COOK: ", end="")
for char in password:
    print(char, end="")
#just for love of linux

This was a start of project, it help alot playng with python during study time, start with necessity of strong password during that time and here it is a every day password generetaor with linux syntax in
hope you like and enjoy as a password generator or simple curiosity or even a point of start for future code, code is fun.
