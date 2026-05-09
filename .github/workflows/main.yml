name: Shadow_Dual_Hani_System
on:
  workflow_dispatch:

jobs:
  farm:
    runs-on: ubuntu-latest
    steps:
      - name: Launch Node 1 (Alpha)
        run: |
          docker run -d honeygain/honeygain -tou-accept -email ${{ secrets.MAIL1 }} -pass ${{ secrets.PASS1 }} -device "Cloud_Alpha_Node"
      - name: Launch Node 2 (Beta)
        run: |
          docker run -d honeygain/honeygain -tou-accept -email ${{ secrets.MAIL2 }} -pass ${{ secrets.PASS2 }} -device "Cloud_Beta_Node"
