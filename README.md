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

----
To configure pip to include the custom repo, create a pip.conf file at: `~/.config/pip/pip.conf` and insert the following:  

```
[global]
extra-index-url = https://radiusai.github.io/
```

If you're sure this file doesn't already exist, this command can be used:  
`mkdir -p ~/.config/pip/ && printf "[global]\nextra-index-url = https://radiusai.github.io/" > ~/.config/pip/pip.conf`  

----


If you see:
Username for 'https://github.com':

Then you may not have HTTPS authentication setup for github.com.

For Mac you can use the osxkeychain: `git config --global credential.helper osxkeychain`
Use your RAI github username and Personal Access Token. These credentials should be store for the future.
