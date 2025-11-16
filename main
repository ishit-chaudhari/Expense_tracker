import datetime

def add_expense():
    print("Add Expense")
    expense = input("Enter the expense: ")
    reason = input("Enter the reason: ")
    with open("expenses.txt", "a") as f:
        f.write(f"{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')} - ₹{expense} - {reason}\n")
    print("Expense added successfully")

def view_expenses():
    print("View Expenses")
    with open("expenses.txt", "r") as f:
        for line in f:
            print(line.strip())

    
def main():
    while True:
        print("Welcome to the Expense Tracker")
        print("--------------------------------")
        print("1. Add Expense")
        print("2. View Expenses")
        print("3. Exit")
        print("--------------------------------")
        choice = input("Enter your choice: ")
        if choice == "1":
            add_expense()
        elif choice == "2":
            view_expenses()
        elif choice == "3":
            break
        else:
            print("Invalid choice")
            continue

if __name__ == "__main__":
    main()
