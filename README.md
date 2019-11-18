# Azure tools
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

    alias azd='docker run -it --rm -v "$(pwd):/work" -v ~/.azure:/work/.azure  pzalews/aztools'

and next you could use:


    azd az login

    azd az resource list


