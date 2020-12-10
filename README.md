# Moulieshproject
nown_user=[]

while True:
    print("hi! i'm travis...")
    name=input('what is your name?:').strip().lower()

    if name in known_user:
        print("hello {} you r already exist in this list...".format(name))
        remove=input("would u like to remove your name formthe list (y/n)?..").lower()
        if remove=='y':
            known_user.remove(name)
            print("<<updated list>>",known_user)
        else:
            add=input("would u like to add this name again (y/n)?:").strip().lower()
            if add=='y':
                known_user.append(name)
                print("<<updated list>>",known_user)
            else:
                print("good to hear..")



    else:
        print("your name is not recoganized!")
        uppdated=input("would u like add your name in list (y/n)?..").lower()

        if uppdated=='y':
            known_user.append(name)
            print("<<updated list>>",known_user)
        else:
            print("we always wait for u ..")
