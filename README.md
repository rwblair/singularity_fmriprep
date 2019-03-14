# fmriprep singularity images
Committing to this repo trigger an autobuild of a singularity image from a docker image. 

To autobuild latest, enter a comment in [Singularity.latest].
To build specific versions/tags, simply create a new Singularity.[tag] file, and make sure to edit the contents.

``` 
From: REPO/IMAGE:[tag/version]
```

Find recent builds here:https://hub.docker.com/r/poldracklab/fmriprep/tags

To download the singularity image after build, run
```
docker run --rm -it -v $PWD/:/root/.singularity/shub/:rw vanessa/sregistry-cli pull shub://kasbohm/singularity_fmriprep[TAG]

```
