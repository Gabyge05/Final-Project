
import json
data = json.load(open('cookrecipes.json'))

def get_cookrecipe(word):
    return data[word]

def menu():
    print("[1] Spanish Paella")
    print("[2] Indian Butte Chicken")
    print("[3] Chinese Yangzhou Fried Rice")
    print("[4] Korean Bibimbap")
    print("[5] Thai Pad Thai")
    print("[0] Exit")

menu()
user_selection = input('What recipe around the world would you like to try?')

while user_selection != 'Exit':
    if user_selection == 'Spanish Paella':
        print(get_cookrecipe(user_selection))
    elif user_selection == 'Indian Butter Chicken':
        print(get_cookrecipe(user_selection))
