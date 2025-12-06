def view_books():
    if not library:
        print("No books in the library yet.")
        return
    
    print("\n--- List of Books ---")
    for idx, book in enumerate(library, 1):
        status = "Available" if book["is_available"] else "Borrowed"
        print(f"{idx}. Title: {book['title']}")
        print(f"   Author: {book['author']}")
        print(f"   Status: {status}")