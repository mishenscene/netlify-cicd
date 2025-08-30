## Deploying an Application via GitHub Actions

### Notes

#### Installing packages

```shell
# Install packages
npm i
```

```shell
# Run application on localhost
ng serve
```

```shell
# Compile the application
ng build
```

The output file is under this dir - Output location: /Users/michelim/workshops/countingbook/dist/countingbook

Deploy the compiled application to Netlify
```shell
# Authenticate netlify credentials
sudo netlify login
```

```shell
sudo netlify build
```

```shell
sudo netlify init
```

```shell
brew install act
```

```shell
# Runs application locally instead of manually setting up docker environment
act
```

```shell
# Deploy in production environment
sudo netlify deploy --prod --dir=dist/countingbook
```

Store credentials in secrets on Github
Settings -> Projects -> Secrets and variables -> Add Repository Secrets
- NETLIFY_AUTH_TOKEN (personal_access_token)
- NETLIFY_SITE_ID (project_id)

Generate a personal access token
Search "personal access token" -> Generate

Locate site ID
Click on netlify linked project -> Project Configuration -> Project ID

```shell
# Checks the secret dir .secrets
act --help | grep secret
```

## Concepts
Bond script &&, execute the first operation.
IF the operation is successful, execute the next operation
Success is determined based on exit code, e.g. 0 == SUCCESS

## Links
