# Getting Data

There are 2 options to get the data:
1. Getting all the data in one batch:
    In order to get data, you need to use the `db` variable that you used at the last section ([Authenticating](https://matan15.github.io/microbiome-data-management-docs/authenticating.html)):

    ```Python
    # Getting documnets as a generator
    docs = db.collection("microbiome").stream()
    ```
    
    The `docs` variable is a generator object, so, you need to iterate it with for loop, for example:
    ```Python
   # Iterating through the documents
    for doc in docs:
        print(f"{doc.id} => {doc.to_dict()}")
    ```

2. Getting all the data in multiple batches (pagination):
    First you need to set the batch size and the collection name:
    ```Python
   # Getting documnets as a generator with page size 100
   docs = db.collection("microbiome").list_documents(page_size=100)
    ```
    In this example, the batch size is 100.
    Then we can iterate through the docs:
    ```Python
   # Iterating through the documents
    for doc in docs:
        print(f"{doc.id} => {doc.get().to_dict()}")
    ```

Note: document with no coordinates, the field `Coordination` won't appear in the document. The rest of the fields that will be empty, their values will be `None`.

For more Information about getting data from Google cloud, you can visit in this link:
[Getting data from Google Firestore](https://cloud.google.com/firestore/docs/query-data/get-data)