1️⃣ gcloud auth login

Logs you (the human) into the gcloud CLI.

Opens a browser → asks you to pick your Google account → stores credentials in:

~/.config/gcloud/credentials.db


Used when you type commands like:

gcloud compute instances list
gcloud storage buckets create my-bucket


👉 Think of it as “login for the CLI tool.”

2️⃣ gcloud auth application-default login

Also opens a browser to log in,

But stores credentials in a different file:

~/.config/gcloud/application_default_credentials.json


These credentials are used by programs and libraries that need access to Google Cloud APIs, including:

Terraform

Google Cloud SDKs (Python, Go, Java, etc.)

👉 Think of it as “login for apps/tools using Google APIs.”