# awscli-docker
All tools need to work with Azure and AKS 

Azure CLI + terraform + kubectl as docker

## INSTALLED TOOLS:
- az cli
- terraform
- kubectl
- yq

## USAGE 

### ACCESS 

Using Azure credentials (az login):

    docker run -it --rm -v "$(pwd):/work" -v ~/.azure:/work/.azure pzalews/aztools terraform --version


### SUGGESTIONS

use alias for bash (or other shell that you are using)

example: 

    alias awsd='docker run -it --rm -v "$(pwd):/aws" -v ~/.aws:/aws/.aws:ro -e AWS_PROFILE=had-dev pzalews/awscli'

and next you could use:

    awsd terraform init
