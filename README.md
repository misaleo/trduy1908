
<!--START_SECTION:badges-->

name: Update badges

on:
  schedule:
    # Runs at 2am UTC
    - cron: "0 2 * * *"
jobs:
  update-readme:
    name: Update Readme with badges
    permissions:
      contents: write
    steps:
      - name: Badges - Readme
        uses: misale/README@main
        with:
          CREDLY_USER: Nguyen-Truong-Duy
          CREDLY_SORT: RECENT
          BADGE_SIZE: 110


<!--END_SECTION:badges-->
