# deploy-flip-forge

Template repository for generating a flipbook from a PDF file with flip-forge and 
deploying it to GitHub pages.

##  How to use:

1. Click on "Use this template" in the top right to generate a new repo for your flipbook
2. After the new repo is created, go to Settings -> Pages
3. Change the "Source" option from "Build from branch" to "GitHub Actions"
4. Upload your PDF to the repository, optionally removing/replacing the existing 
   "book.pdf" one.
5. Edit [.github/workflows/deploy.yml](.github/workflows/deploy.yml) file and change 
   the following options as needed. Make sure that at least the "file" is set to the 
   correct PDF file name:
   ```yaml
   with:
     file: "book.pdf"
     title: "Book title"
     backgroundColor: "#000000"
     toolbarColor: "#ffffff"
     description: "Book description"
   ```
6. Go to the "actions" tab and wait until the deployment action completes.
7. Visit the generate GitHub page and in order to see your new flipbook. 
   The link should look something like https://USERNAME.github.io/REPOSITORY/
