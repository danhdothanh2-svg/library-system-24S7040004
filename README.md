def add_book():
    title = input("Enter book title: ").strip()
    author = input("Enter author: ").strip()
    if title and author:
        book = {
            "title": title,
            "author": author,
            "is_available": True
        }
        library.append(book)
        print("Book added successfully!")
    else:
        print("Title and author cannot be empty!")
