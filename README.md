# lubbockhamradio
![Build & Deploy](https://github.com/cliffcolvin/lubbockhamradio/actions/workflows/hugo.yaml/badge.svg)

The Lubbock, TX ham radio community is a wide spread and vastly diverse group of people and interests. This website [LubbockHamRadio.org](https://lubbockhamradio.org) is meant to give that community a central place to aggregate the happenings in the community.

Any person that is interested in radio in Lubbock is welcome to contribute to this website and I'll work to merge those PRs as often as possible.

# Setup to contribute
- [Install hugo](https://gohugo.io/installation/)
- (Recommended) [Download VS Code](https://code.visualstudio.com/download) for text editing the markdown 
- All pages and posts are written in markdown, use [Markdown cheat sheet](https://www.markdownguide.org/cheat-sheet/) to learn more.
- [Create a github account](https://github.com/join)
- [Install git](https://github.com/git-guides/install-git)
- [Clone the repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)

# Create a branch for your post
In the command prompt you will need to change directory to the place you cloned the repository above.

Then create a branch
`git branch my-post-name`

# Adding Content

Type a command to create the post file
`hugo new content posts/friendly-post-name.md`

Open the file you just created in vs code and edit the markdown to add your post content.

In the header section between the three +++ pluses you will see the post meta data.
```
+++
title: "My First Post"
date: 2022-11-20T09:03:20-08:00
draft: true
+++
```

Edit your title and set draft to false

```
+++
title: "My Post title"
date: 2022-11-20T09:03:20-08:00
draft: false
+++
```


Below that add your markdown for the post content.

# Submitting your addition

Once complete you will need to submit your changes and raise a pull request.

In the command prompt run
`git commit -a -m my commit message with a post title`
Then push 
`git push`

Next go to the [github repository pull requests](https://github.com/cliffcolvin/lubbockhamradio/pulls) and you should see a message saying that you pushed a branch and giving the option to raise a pull request.

Once this is done our maintainers will review and merge. After merge the site will be automatically updated.


# Running and testing the site locally

To run the site locally you can use the following command
`hugo server`

When that completes running you can browse to [http://localhost:1313](http://localhost:1313/) in your web browser and browse to your new post. This will allow you to test and edit your post before requesting it to be published.