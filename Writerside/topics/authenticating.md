# Authenticating

If you got the credentials from the cloud administrator, you can authenticate with Google cloud:

```Python
from google.oauth2 import service_account
from google.cloud import firestore

###########################################

# getting credentials as dictionary

###########################################

# Creating credentials object
credentials = service_account.Credentials.from_service_account_info(creds_from_json)

# Connecting to the database
db = firestore.Client(
    project=creds_from_json["project_id"],
    credentials=credentials,
    database="microbiome"
)

```

