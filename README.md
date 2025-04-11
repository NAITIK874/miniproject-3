import random

def pick_random_choice(choices):
    if not choices:
        return "No choices provided."
    return random.choice(choices)

# Example usage
print("Enter your choices separated by commas:")
user_input = input("> ")
choices = [choice.strip() for choice in user_input.split(",")]

selected = pick_random_choice(choices)
print(f"\n🎉 Randomly selected: {selected}")
