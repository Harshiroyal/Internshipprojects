# Internshipprojects[to-do application development.pdf](https://github.com/Harshiroyal/Internshipprojects/files/13335515/to-do.application.development.pdf)

tasks = {}

def display_menu():
    print("\nTODO LIST APPLICATION")
    print("1. Add Task")
    print("2. View Tasks")
    print("3. Mark Task as Completed")
    print("4. Exit")

def add_task():
    task_name = input("Enter the task: ")
    tasks[task_name] = False
    print("Task added successfully!")

def view_tasks():
    print("\nTASKS:")
    for task, completed in tasks.items():
        status = "Completed" if completed else "Not Completed"
        print(f"- {task} ({status})")

def mark_completed():
    view_tasks()
    task_name = input("Enter the task to mark as completed: ")
    
    if task_name in tasks:
        tasks[task_name] = True
        print("Task marked as completed!")
    else:
        print("Task not found.")

while True:
    display_menu()
    choice = input("Enter your choice (1-4): ")

    if choice == "1":
        add_task()
    elif choice == "2":
        view_tasks()
    elif choice == "3":
        mark_completed()
    elif choice == "4":
        print("Exiting the application. Goodbye!")
        break
    else:
        print("Invalid choice. Please enter a number between[to-do application development.pdf](https://github.com/Harshiroyal/Internshipprojects/files/13335520/to-do.application.development.pdf)
