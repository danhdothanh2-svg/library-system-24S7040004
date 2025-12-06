def search_book():
    if not library:
        print("Library is empty.")
        return
        
    query = input("Enter keyword to search in title: ").strip().lower()
    found = False
    print("\n--- Search Results ---")
    for idx, book in enumerate(library, 1):
        if query in book["title"].lower():
            status = "Available" if book["is_available"] else "Borrowed"
            print(f"{idx}. Title: {book['title']}")
            print(f"   Author: {book['author']}")
            print(f"   Status: {status}")
            found = True
    if not found:
        print("No books found matching the keyword.")