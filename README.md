# Building course for Teach The Web

The original version of this course as part of Teach The Web can be found [here](http://training.webmakerprototypes.org/en/building/concepts/)

If you are reading this README, chances are that you are considering running a customized version of this course. This has some technical and idealogical considerations and luckily you are not alone in this! Below are instructions on how to setup the technical bits, but for when you are well on your way or if you get stuck at any point, reach out [on our discussion forum](http://discourse.webmakerprototypes.org/).

## Creating your own version of this course

To start building your own course, you will need to sign up for a github account and then fork this repository. You can do that by clicking the fork button in the top right hand corner. If you do not already have a Github account, you will be asked to sign up and from there you can follow the instructions.

Once you have forked the repository, you will be redirected to your own version of this course. Here you can play and experiment in the safe confines of your own version.

The very first thing you may want to do is update the landing page of this course. You can do so by editing the index.html file in the root of your repository.

The contents of the course is stored in the `_posts` folder. You will notice some info at the top that looks like this:

    ---
    title: <span class="fa fa-random"></span> Concepts
    layout: multicourse_page
    categories: [building]
    ---

Here you can tweak the title of the course by simply editing the text! The `layout` and `categories` fields are used to make things show up in the correct places. If you do some advanced things you may need to change them, but for down down worry too much.

Below the top header you'll find the content of the course modules. They are written in Markdown and you can tweek them to your heart's content!

Changing things like the course title and image can be done by editing the `_data/course.yml` file. The default content should look something like this:

    building:
      title: "Building"
      category: building
      language: en
      fork_url: https://github.com/dirkcuys/ttw-building
      based_on:
      image: /img/building-360px.jpg
      image_attribution: https://secure.flickr.com/photos/debloper/10607673915/in/photostream/
      attribution_name: Soumya Deb

The fields that are of interest is `title` which is the title of the course, `image` which is a link to the course image (seen on the left when you view the course content), `image_attribution` and `attribution_name` which are a link to the image and the creators name respectively if you are using a CC-BY-SA license.

After you've made changes, you can see your version of the site by going to http://yourgithubusername.github.io/ttw-building/! Just replace yourgithubusername with your actual github user name. Because of the way that Github pages works, you will need to make at least one page before you will see the changes. And if it is your first time using github pages, it may take a while for the pages to become live, but don't worry, Github will probably send you an email saying that :)
