```
$ helm lint chart-with-rc
==> Linting chart-with-rc
[INFO] Chart.yaml: icon is recommended
[INFO] values.yaml: file does not exist
[WARNING] templates/: directory not found

1 chart(s) linted, no failures

$ helm lint chart-without-rc
==> Linting chart-without-rc
[INFO] Chart.yaml: icon is recommended
[INFO] values.yaml: file does not exist
[WARNING] templates/: directory not found

1 chart(s) linted, no failures

$ helm lint chart-without-rc-1.0.0.tgz
==> Linting chart-without-rc-1.0.0.tgz
[INFO] Chart.yaml: icon is recommended
[INFO] values.yaml: file does not exist
[WARNING] templates/: directory not found

1 chart(s) linted, no failures

$ helm lint chart-with-rc-1.0.0-rc1.tgz
==> Skipping chart-with-rc-1.0.0-rc1.tgz
No chart found for linting (missing Chart.yaml)

Error: 0 chart(s) linted, 1 chart(s) failed
```
