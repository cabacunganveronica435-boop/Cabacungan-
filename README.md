def describe_pet(animal_type, pet_name):
    print(f"I have a {animal_type} and its name is {pet_name}.")

describe_pet("dog", "Buddy")
describe_pet("cat", "Milo")
describe_pet("rabbit", "Snowy")

print()

describe_pet("dog", "Buddy")
describe_pet(pet_name="Milo", animal_type="cat")

print()

def describe_pet(pet_name, animal_type="dog"):
    print(f"I have a {animal_type} and its name is {pet_name}.")

describe_pet("Brownie")
describe_pet("Nugget", "chicken")

print()

def order_drink(drink, size="medium", iced=False):
    if iced:
        return f"Your order: {size} iced {drink}"
    else:
        return f"Your order: {size} hot {drink}"

print(order_drink("coffee"))
print(order_drink("chocolate", size="large", iced=False))
print(order_drink("milk tea", size="small", iced=True))

print()

def compute(operation, num1, num2=1):
    if operation == "add":
        return num1 + num2
    elif operation == "multiply":
        return num1 * num2
    elif operation == "subtract":
        return num1 - num2
    else:
        return "Invalid operation"

print(compute("add", 5, 10))
print(compute("multiply", num1=3, num2=4))
print(compute("subtract", 20))
print(compute("divide", 10, 2))
