# aci-fastapi-skeleton
this is a single-container-application example.

`app/main.py` is a a fastAPI example python project.

# testing
it doesn't have any yet

https://fastapi.tiangolo.com/tutorial/testing/ at some point

#  container images

github actions builds the images and stores them in azure container image registry.

# deployment

there are two current containers running, `main` & `staging`, but if you create a new branch and let the github action run, you'll see it will launch `gruff-azure-{branch}.westus.azurecontainer.io`.  sometimes DNS can be a little slow. (<5min>)

## staging url
http://gruff-azure-staging.westus.azurecontainer.io/

## main url
http://gruff-azure-main.westus.azurecontainer.io/

since this project doesn't have high performance requirements, azure container instances is perfectly suitable.

once container orchestration is really needed, we can create a kubernetes deployment and use a service router.

https://docs.microsoft.com/en-us/azure/container-instances/container-instances-orchestrator-relationship
