- 👋 Hi, I’m @xczgx
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
xczgx/xczgx is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
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
