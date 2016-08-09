# Module Roundup

Collect information about modules in a given date range.

## Options

####`start_date` (required)

The earliest release publication datetime to include (Example: `2016-07-01`).

####`-o, --output` (optional, default: the value give as `start_date`)

The name of the ouput file. The file will be created in `reports/`.
The default file name is the same string given as the `start_date`

####`-e, --enddate` (optional, default: current date/time)

The latest release publication datetime to include (Example: `2016-08-01`).

## Usage

### Example

This will collect information for all releases for july and write the information
to `reports/july.md`.

```bash
$ bundle exec roundup 2016-07-01 -e 2016-08-01 -o july.md
```

### Help information

```
Collect information about all modules released in a given date range.

Usage:
       roundup [options] start_date

Allowed date formats:
       YYYY-MM-DD

where [options] are all optional:
  -o, --output=<s>     The name of the file that will be created in the report directory (default: the provided start date)
  -e, --enddate=<s>    An end date (don't count modules published after this date.) (default: 2016-08-09T15:53:23-07:00)
  -h, --help           Show this message
```

## Markdown

If you'd like to render the markdown locally, check out [grip](https://github.com/joeyespo/grip).
