# quick overview:
connect to your concourse server with fly-cli

create a credentials.yml file using the cred-template.yml file.

push pipeline:
fly -t <target name> sp -c pipelines/pipeline.yml -p deployment-pipeline --load-vars-from credentials.yml

modify the app in ./webapp
```
git add.
git commit -m "modified webapp"
git push
```
watch the magic happen.

