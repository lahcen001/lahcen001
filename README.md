### Hi there 👋
im full stack web developer ( 
name: Waka Readme

on:
  workflow_dispatch:
  schedule:
    # Runs at every 12AM UTC
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: Update this repo's README
    runs-on: ubuntu-latest
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}

