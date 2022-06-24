# radiusai.github.io

## Usage

This is Python Package Index is a public repository containing only packaging metadata which points at private Github 
repositories using the HTTPS . HTTPS authentication with Github is required and for a seemless pip install experience it 
is advised to add HTTPS github authentication using the [Github Credentials Manager](https://docs.github.com/en/get-started/getting-started-with-git/caching-your-github-credentials-in-git)
and a [Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token).


#### Installing Packages

To install a package from this index you'll need an additional flag with the `pip install` command:  
`--extra-index-url https://radiusai.github.io/`  

So a fully formed command would look something like this:

`pip install retl==0.15.37 --extra-index-url https://radiusai.github.io/`

You can also update to the latest published version:

`pip install retl --upgrade --extra-index-url https://radiusai.github.io/`

To avoid using the extra index url flag you can add an alias for `pip install` named `pip-install`. This is shell dependent:

ZSH: `echo 'alias pip-install="pip install --extra-index-url https://radiusai.github.io/"' >> ~/.zshrc`  
BASH: `echo 'alias pip-install="pip install --extra-index-url https://radiusai.github.io/"' >> ~/.bashrc`


The extra index is checked after the public PyPi repository, so you may call `pip-install` instead of `pip install` for 
all packages if desired:

`pip-install retl`  
`pip-install retl --upgrade`  
`pip-install retl==0.15.37`  
