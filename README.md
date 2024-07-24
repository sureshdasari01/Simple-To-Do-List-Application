# Simple-To-Do-List-Application
Create a Python program for adding, completing, and removing tasks—a simple introduction to Python programming.
here's a simple Python program that demonstrates how to add, complete, and remove tasks. This program uses a basic command-line interface and stores tasks in a list.

python
# Simple Task Manager in Python

def display_menu():
    print("\nTask Manager")
    print("1. Add Task")
    print("2. Complete Task")
    print("3. Remove Task")
    print("4. View Tasks")
    print("5. Exit")

def add_task(tasks):
    task = input("Enter the task: ")
    tasks.append({'task': task, 'completed': False})
    print(f"Task '{task}' added.")

def complete_task(tasks):
    view_tasks(tasks)
    task_num = int(input("Enter the task number to complete: ")) - 1
   
