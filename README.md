# azure-serverless-fastapi-containers-skeleton
this is a single-container-application example.

`app/main.py` is a a fastAPI example python project.

# testing
it doesn't have any yet

https://fastapi.tiangolo.com/tutorial/testing/ at some point

# deployment

there are two current containers running, `main` & `staging`, but if you create a new branch and let the github action run,

you'll see it will launch `gruff-{branch}-backend.westus.azurecontainer.io`.  sometimes DNS can be a little slow.

## main / production url
http://gruff-azure-main.westus.azurecontainer.io/

## staging url
http://gruff-azure-staging.westus.azurecontainer.io/

