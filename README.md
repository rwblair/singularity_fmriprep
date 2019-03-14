# fmriprep singularity images
Committing to this repo trigger an autobuild of a singularity image from a docker image. 

To autobuild latest, enter a comment in [Singularity.latest](Singularity.latest)
To build specific versions/tags, simply change the Singularity.[tag], and make sure to change the tag in the file as well.

``` 
From: REPO/IMAGE:[tag/version]
```

Find recent builds here:https://hub.docker.com/r/poldracklab/fmriprep/tags

Images are built at https://www.singularity-hub.org/collections/2529, and can be downloaded by running
```
docker run --rm -it -v $PWD/:/root/.singularity/shub/:rw vanessa/sregistry-cli pull shub://kasbohm/singularity_fmriprep[TAG]

```
