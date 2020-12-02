# Dev Delta Jokes

##### This repository will contain everyone's different joke websites from lesson 2. We will use it to learn Git and GitHub, and to work collaboratively!

###### [Check out the live site](https://developer-delta.github.io/dev-delta-jokes/)

## Getting your site into this repo:
* Use `git clone` to pull this repository down to your local machine.
* `cd` into the newly cloned directory.
* Use the `git checkout -b` command to create a _new branch_ for the changes you will be making. 
  * _You can name it whatever you like, but descriptive branch names are always good! Maybe something like `kylos-website-addition`._
    <details>
    <summary>Code</summary>

      ```shell
      # the -b flag stands for "branch", as in you are creating a new branch with this name
      git checkout -b kylos-website-addition
      ```
    </details>
* Create a directory (`mkdir`) in the base folder titled `your-name`.
  ![Screen Shot of the terminal command "mkdir kylo"](https://i.imgur.com/pyyRgIE.png)
* Run `ls` to make sure your new folder is there.
  ![Screen Shot of the ls terminal command outputting a list of directories and files, one of which is the newly created directory "kylo"](https://i.imgur.com/LcTpvRB.png)
* Copy over your `html` and `css` files from your joke website CSS homework into your newly created directory.
* Next you'll need to make a change to the `index.html` file in the root of this repo.
  * Add a placeholder list item to edit inside the `ul` element.
  * Inside your chosen list item, add an anchor tag that links to your `html` file for your joke website.
  * Add some text to your anchor tag so the users have a descriptive hyperlink to click on.

### Takeaways from contributing to this repository:
* You will be able to learn from others work, and get feedback on yours by using `pull requests`.
* Your website will be `deployed` onto the web as a part of this repo.
* Your first dive into `open source` software!
* 