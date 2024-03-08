# Getting Data

In order to get data, you need to use the `db` variable that you used at the last section ([Authenticating](https://matan15.github.io/microbiome-data-management-docs/authenticating.html)):

```Python
docs = db.collection("microbiome").stream()
```

The `docs` variable is a generator object, so, you need to iterate it with for loop, for example:
```Python
for doc in docs:
    print(f"{doc.id} => {doc.to_dict()}")
```