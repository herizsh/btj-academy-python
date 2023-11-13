# Notes App

Create a basic note App using Python.
Allow users to add, view, and delete notes.
Store the notes in a text file for persistent storage.

```md
Welcome to the Simple Note App!

Menu:
1. Add Note
2. View Notes
3. Delete Note
4. Exit

Enter your choice (1-4): 1
Enter your note: This is a sample note.

Note added successfully.

Menu:
1. Add Note
2. View Notes
3. Delete Note
4. Exit

Enter your choice (1-4): 2
Your Notes:
1. This is a sample note.

Menu:
1. Add Note
2. View Notes
3. Delete Note
4. Exit

Enter your choice (1-4): 3
Your Notes:
1. This is a sample note.

Enter the number of the note to delete: 1
Note deleted successfully.

Menu:
1. Add Note
2. View Notes
3. Delete Note
4. Exit

Enter your choice (1-4): 2
No notes found.

Menu:
1. Add Note
2. View Notes
3. Delete Note
4. Exit

Enter your choice (1-4): 4
Exiting the Note App.
```

## Boilerplate Code

```python

def add_note():
    note = input("Enter your note: ")
    # Code Here

    print("Note added successfully.")

def view_notes():
    print("Your Notes:")
    # Code Here

def delete_note():
    view_notes() # Before
    # Code Here
    print(f"Note deleted successfully.")
    view_notes() # After Delete

while True:
    print("\nMenu:")
    print("1. Add Note")
    print("2. View Notes")
    print("3. Delete Note")
    print("4. Exit")

    choice = input("Enter your choice (1-4): ")

    if choice == "1":
        add_note()
    elif choice == "2":
        view_notes()
    elif choice == "3":
        delete_note()
    elif choice == "4":
        print("Exiting the Note App.")
        break
    else:
        print("Invalid choice. Please enter a number between 1 and 4.")

```
