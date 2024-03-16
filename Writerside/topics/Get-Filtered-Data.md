# Get Filtered Data

in order to get filtered data, we need to import additional Class from Google Firestore: `FieldFilter`

```Python
from google.cloud import firestore
from google.cloud.firestore import FieldFilter
```

After [Authenticating](https://matan15.github.io/microbiome-data-management-docs/authenticating.html), we need to select which collection we want to use:
```Python
# Connecting to the collection
docs = db.collection("microbiome")
```

And then, in order to filter the docs, we will use the `FieldFilter` that we imported before, The `FieldFilter` Class takes three parameters: a field to filter on, a comparison operator, and a value:
```Python
# Filter documents
filtered_docs = docs.where(filter=FieldFilter("field name", "oprator", "value"))

# Iterate through the filtered documents
for doc in docs.stream():
    print(f"{doc.id} => {doc.to_dict()}")
```

For example, if we want to get all the Fungi samples, we will write:
```Python
# Filter the documents with Kingdom "Fungi"
filtered_docs = docs.where(filter=FieldFilter("Kingdom", "==", "Fungi"))

for doc in docs.stream():
    print(f"{doc.id} => {doc.to_dict()}")
```

Another example, if we want to get all the Bacteria samples, we will write:
```Python
# Filter the documents with Kingdom "Bacteria"
filtered_docs = docs.where(filter=FieldFilter("Kingdom", "==", "Bacteria"))

for doc in docs.stream():
    print(f"{doc.id} => {doc.to_dict()}")
```

There are more operators that you can use, Firestore supports the following comparison operators:
* `<` less than
* `<=` less than or equal to
* `==` equal to
* `>` greater than
* `>=` greater than or equal to
* [`!=` not equal to](https://cloud.google.com/firestore/docs/query-data/queries#not_equal)
* [`array-contains`](https://cloud.google.com/firestore/docs/query-data/queries#array_membership)
* [`array-contains-any`](https://cloud.google.com/firestore/docs/query-data/queries#in_and_array-contains-any)
* [`in`](https://cloud.google.com/firestore/docs/query-data/queries#in_and_array-contains-any)
* [`not-in`](https://cloud.google.com/firestore/docs/query-data/queries#in_and_array-contains-any)

You can read more about filtering data [here](https://cloud.google.com/firestore/docs/query-data/queries).
