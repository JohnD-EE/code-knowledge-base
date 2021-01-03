# Computed Properties
A way to define a data property inside the component, that depends upon other data in the component.

E.g. might want to create a filtered array of a larger object.

Imagine you have an array of books:
```
books: [
	{ title: 'name of book 1', isFav: true },
	{ title: 'name of book 2', isFav: false },
	{ title: 'name of book 3', isFav: true },
]
```

We could make a computed property using the JavaScript `filter` function thus:
```
computed: {
	filteredBooks() {
		return this.books.filter((book) => book.isFav)
	}
}
```

