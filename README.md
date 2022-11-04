# download-file
Github action to download a file with wget that works on a multi-platform runners

```yaml
inputs:
  url:
    description: 'The url to download the file from'
    required: true
```

## Usage:

```yaml
steps:
- uses: peternied/download-file@v1
  with:
    url: https://raw.githubusercontent.com/peternied/download-file/main/README.md

- name: Use downloaded file
  run: cat README.md
```
