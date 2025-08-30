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
# Deploy in production environment
sudo netlify deploy --prod --dir=/dist/countingbook/browser
```

```shell
brew install act
```

```shell
# Runs application locally instead of manually setting up docker environment
act
```

Bond script &&, execute the first operation.
IF the operation is successful, execute the next operation
Success is determined based on exit code, e.g. 0 == SUCCESS

## Links
