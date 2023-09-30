# JFROG
Initial script uploaded is for artifactory cleanup script-JFROG

To retrieve a list of all artifacts in a repository using the Artifactory Query Language (AQL) via the RESTful API, you can use the following curl command:

query.aql--Identifies artifacts not downloaded 30Days ago
You can run  curl against query.aql --> */
------>curl -u USERNAME:API_KEY_OR_PASSWORD -X POST "https://YOUR-ARTIFACTORY-URL/artifactory/api/search/aql" -H "Content-Type: text/plain" -T query.aql 
/*
**Note-->If you have an ssl error or tls,, use -k or --insecure tag to skip this warning.**





# JFROG -- Artifactroy cleanup automation
To automate the process of deleting artifacts in an Artifactory repository without manually specifying the repository name each time, you can create a script that iterates through all repositories and deletes artifacts that match your criteria. run the artifactory-cleanup.py
