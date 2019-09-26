# Hello world docker action

This action prints "Hello World" or "Hello" + the name of a person to greet to the log.

## Inputs

### `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.

## Outputs

### `time`

The time we greeted you.

## Example usage

uses: actions/hello-world-docker-action@v1
with:
  who-to-greet: 'Wasim'

## Testing it out

Locally, check that we can build and run the Docker container.

```
docker build -t echo-container .

docker run echo-container world 
```

and we should see:

```
Hello world
::set-output name=time::Thu Sep 26 08:15:49 UTC 2019
```



