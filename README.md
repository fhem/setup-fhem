# setup-fhem
Github action that simpifies setup of fhem in a Workflow for testing or other purpose

Currently this action supports installation of fhem via debain nightly package

## Inputs

### `mode`

**Optional** The installation mode fhem. Currently only `debian` is supported. Default is `debian`

### `runservice`

**Optional** Should the standard service, which is started by the debian package be running? Normaly this is not needed. Default is `false`


## Outputs

Currently there are not outputs provided

## Example usage
1. Checkout the repository

```
    steps: 
    - name: Checkout Repostory
      uses: actions/checkout@v3
```

2. You can create the controls file
```
    - name: Install FHEM via debian nightly 
      uses: fhem/setup-fhem@v1.0.0
```

... Now you can run automated tests or whatever you want to do
