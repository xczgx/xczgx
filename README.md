- š Hi, Iām @xczgx
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
xczgx/xczgx is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
name: Run MATLAB Tests on Self-Hosted Runner
on: [push]
jobs:
  my-job:
    name: Run MATLAB Tests
    runs-on: self-hosted
    steps:
      - name: Check out repository
        uses: actions/checkout@v2
      - name: Run tests
        uses: matlab-actions/run-tests@v1
