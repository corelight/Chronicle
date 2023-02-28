# Chronicle CBN Tool

Command line tool to interact with Chronicle's Config Based Normalizer APIs.

Config Based Normalizer (CBN) APIs allow customers to manage config based
parsers that normalize logs published to Chronicle. This script provides a
command line tool to interact with CBN APIs and manage config based parsers.

## Setup

Follow these instructions: https://cloud.google.com/python/setup

You may skip installing the Cloud Client Libraries and the Cloud SDK, they are
unnecessary for interacting with Chronicle.

After creating and activating the virtual environment `venv`, install Python
library dependencies by running this command:

```shell
pip install -r requirements.txt
```

It is assumed that you're using Python 3.6 or above.

## Credentials

Running the samples requires a JSON credentials file. By default, all the
samples try to use the file `.chronicle_credentials.json` in the user's home
directory. If this file is not found, you need to specify it explicitly by
adding the following argument to the sample's command-line:

```shell
--credentials_file <path>
```

## Usage

- Getting Sample Logs
```shell
./cbn_cli.py --credentials_file=~/.chronicle_credentials.json gen --log_type=CORELIGHT --start_date=2023-03-01T00:00:00Z --end_date=2023-03-15T12:00:00Z
```

- Running Validation
```shell
python cbn_cli.py --credentials_file=~/.chronicle_credentials.json run --conf_file=../CORELIGHT.conf --log_file=corelight.log  > validate.txt
```

- Download a parser
```shell
python cbn_cli.py --credentials_file=~/.chronicle_credentials.json download --config_id=CORELIGHT
```

- Submitting a new parser
```shell
python cbn_cli.py --credentials_file=~/.chronicle_credentials.json submit --conf_file=../CORELIGHT.conf --log_type=CORELIGHT --author=james.lagermann@corelight.com
```

- Getting status of a submitted parser
```shell
python cbn_cli.py --credentials_file=~/.chronicle_credentials.json status --config_id=aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa
```

- Getting history of a given parser
```shell
python cbn_cli.py --credentials_file=~/.chronicle_credentials.json history --log_type=CORELIGHT
```

- List all parsers of a given customer
```shell
python cbn_cli.py --credentials_file=~/.chronicle_credentials.json list
```

- List errors of a log_type between specific timestamps
```shell
python cbn_cli.py --credentials_file=~/.chronicle_credentials.json err --start_date=2023-03-01T00:00:00Z --end_date=2023-03-15T12:00:00Z --log_type=CORELIGHT
```
