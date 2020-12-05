# Dev Delta Jokes

##### This repository will contain everyone's different joke websites from lesson 2. We will use it to learn Git and GitHub, and to work collaboratively!

##### [Check out the live page](https://developer-delta.github.io/dev-delta-jokes/) with everyone's websites!

---

## Getting your site into this repo:
* Use `git clone` to copy this repository down to your local machine.
  <details>
  <summary>Code</summary>

    ```shell
    git clone https://github.com/developer-delta/dev-delta-jokes.git
    ```
  </details>

>

* `cd` into the newly cloned directory.
  <details>
  <summary>Code</summary>

    ```shell
    cd dev-delta-jokes
    ```
  </details>

>

* Use the `git checkout -b` command to create a _new branch_ for the changes you will be making. 
  <details>
  <summary>Code</summary>

    ```shell
    # the -b flag stands for "branch", as in you are creating a new branch with this name
    git checkout -b kylos-website-addition
    ```
  </details>

  > _You can name it whatever you like, but descriptive branch names are always good!_

>

* Create a directory (`mkdir`) in the base folder titled `your-name`.

  <details>
  <summary>Code</summary>

    ```shell
    # in the directory "dev-delta-jokes"
    mkdir kylo
    ```
  </details>

>

* Run `ls` to make sure your new folder is there.

  ![Screen Shot of the ls terminal command outputting a list of directories and files, one of which is the newly created directory "kylo"](https://i.imgur.com/LcTpvRB.png)

> 

* Copy over your `html` and `css` files from your joke website CSS homework into your newly created directory.

  <details>
  <summary>Code</summary>

    ```shell
    cp location/of/your/joke/site/index.html kylo
    ```

    ```shell
    cp location/of/your/joke/site/main.css kylo
    ```
  </details>

>

* Next you'll need to make a change to the `index.html` file in the root of the repo.
  * Find your name in the placeholder list items to edit inside the `ul` element.
  * Inside your list item, add an anchor tag that links to your `html` file for your joke website.
    <details>
    <summary>Code</summary>

      ```html
      <li><a href="kylo/index.html">Kylo's joke page</a></li>
      ```
    </details>

> 

* After we are done making our changes, we need to `git add` our files, and `git commit` them to be all bundled up and ready to go to GitHub. _we can pass directories to `git add` to add everything inside_
  <details>
  <summary>Code</summary>

    ```shell
    git add kylo/
    ```

    ```shell
    git add index.html
    ```

    ```shell
    # -m stands for "message", so "commit these changes with this message"
    git commit -m "my first commit"
    ```
  </details>

>

* Now that you have committed (saved) your changes locally on your _own branch_ of this repo, you need to _push_ that branch up to GitHub using `git push`!
  <details>
  <summary>Code</summary>

    ```shell
    git push
    ```

    Hmm... that probably didn't work for you either, huh? The reason is that you created that branch only on your local machine! GitHub has no idea that it exists, so we need to tell it about it and then we can push it up! _We even got some helpful output from Git telling us what to do!_

    ```shell
    git push --set-upstream origin kylos-website-addition
    ```

    > In that command, "upstream" means on GitHub/the internet, and "origin" is saying this is the name of the GitHub home for my new branch

  </details>

> 

* Alright!! Now we just need to create a __pull request__ to say _"hey I want to __merge__ my code (on my branch) back into the big main repository (master branch) so I can see my changes on the internet!"_
  * This part we will do in GitHub itself. So [open up the `dev-delta-jokes` repository on GitHub](https://github.com/developer-delta/dev-delta-jokes).
  * If you click on the button that says `master`, that's for "master" branch, you should see __your__ branch listed underneath there! Go ahead and click on it.
  
    ![Screen Shot of the "master" branch button dropdown on GitHub](https://i.imgur.com/DLhvcdm.png)

  * Now we are viewing our branch in the UI of GitHub. To the right a little bit is a `Pull request` button we can go ahead and click on now.

    ![Screen Shot 2020-12-04 at 3.56.57 PM](https://i.imgur.com/ExmFATv.png)
  
  * Now you should see a page noting that there are differences between the `master` branch and your branch. This is expected because we made some changes to add our website and the link to it to this repository. So now go ahead and click `Create pull request`!

  * What happens next is your Pull request will be reviewed by whoever is the maintainer of the repository, and they may make comments on your pull request, or approve and merge it in! When it is merged in, your changes will "go live" and you'll be able to see your work on the live website!

---

![Rick and Morty celebrating](https://media1.tenor.com/images/5bb201883ea639c256f5928b77466a9d/tenor.gif)

Congrats on your first foray into `open source` software!