# Digital Garden

A CLI tool for the creation and maintenance of Digital Gardens.

## Commands

### Setting the garden path

```shell
GARDEN_PATH=~/github/my-digital-garden garden write
garden -p ~/github/my-digital-garden write
garden --garden_path ~/github/my-digital-garden write
```

### write

Open a new file to write in our digital garden. Since we don't necessarily konw what we want
to title what we're writing, we'll leave the title as optional and ask the user for it later
if they don't provide it up front.

```shell
garden write
garden write -t "Some Title"
```

## Development

### Testing
NOTE: tests depend on a shell script being executable by the test framework. If tests fail, ensure that `./tests/fake-editor.sh` has executable permissions by running `ls -l` in the 


```shell
cargo test
```