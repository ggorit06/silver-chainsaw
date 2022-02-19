# silver-chainsaw

# task: estimating the risk of death from coronavirus


def getBoolean(input_str: str):
    """
    Returns a boolean value from a string
    """
    if input_str.lower() in ("yes", "y"):
        return True
    elif input_str.lower() in ("no", "n"):
        return False
    else:
        print("You did not enter a valid answer")
        exit()


age = input("Are you a cigarette addict older than 75 years old? (yes/no)\n")
age = getBoolean(age)

chronic = input("Do you have a severe chronic disease? (yes/no)\n")
chronic = getBoolean(chronic)

immune = input("Is your immune system too weak? (yes/no)\n")
immune = getBoolean(immune)

if age or chronic or immune:
    print("You are in risky group")
else:
    print("You are not in risky group")
