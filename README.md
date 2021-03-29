# rmziplock

This bash script removes a known password from an encrypted ZIP file.

## Installation

Use the following command to install this software:

```bash
$ make
$ make install
```

The default `PREFIX` is set to `/usr/local`.  In order to succesfully complete the installation, you need to have write permissions for the installation location.

## Usage

The following command will extract the contents of the encrypted zipfile to a temporary folder and create a new zipfile without password encryption.  The password needs to be entered interactively by the user.


```bash
$ rmziplock [options] file[.zip]
```

### Options

+ `-o`

  Sets the name of the output file.  If omitted, the suffix `_unlocked` will be appended to the basename of the encrypted ZIP file.

+ `-y`

  Permission to overwrite existing files.

+ `-h`

  Shows this help message.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
