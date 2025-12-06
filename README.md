# library.py
library = []  # Danh sách toàn cục lưu sách
def main():
    while True:
        print("\n--- LIBRARY MANAGEMENT SYSTEM ---")
        print("1. Add New Book")
        print("2. View All Books")
        print("3. Search Book")
        print("4. Exit")
        choice = input("Enter your choice: ")

        if choice == "1":
            add_book()
        elif choice == "2":
            view_books()
        elif choice == "3":
            search_book()
        elif choice == "4":
            print("Exiting program.")
            break
        else:
            print("Invalid choice. Please try again.")
def add_book():
    pass  # sẽ implement ở feature sau
def view_books():
    pass
def search_book():
    pass
if __name__ == "__main__":
    main()