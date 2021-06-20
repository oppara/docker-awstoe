# docker-awstoe

[Develop AWS TOE components locally - EC2 Image Builder](https://docs.aws.amazon.com/imagebuilder/latest/userguide/image-builder-component-manager-local.html)


## usage

validate
```
$ docker run --rm \
-v $(pwd):/data \
-w /data oppara/awstoe \
awstoe validate \
--documents /path/to/components.yaml
```

run
```
$ docker run --rm \
-v $(pwd):/data \
-w /data oppara/awstoe \
awstoe run \
--documents /path/to/components.yaml \ 
--phases build
```