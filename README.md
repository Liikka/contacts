
def DeleteContact():
    name = input('Enter name: ')
    found = False

    for contact in contacts:
        if contact['name'] == name:
            contacts.remove(contact)
            found = True
            break

    if found:
        print(f"Contact {name} has been deleted.")
    else:
        print(f"Contact {name} not found.")
