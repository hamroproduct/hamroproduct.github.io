# hamroproduct.github.io
hamroproduct.com

# Guide

1. Download and install Hugo

  *Archlinux*

  ```bash
    $ yaourt -S hugo
  ```

  *Debian / Ubuntu / other linux*

  From [https://github.com/spf13/hugo/releases](https://github.com/spf13/hugo/releases) download .deb (or .rpm, or distos package) file into ~/Downloads folder

  ```
    $ cd ~/Downloads
    $ sudo dpkg -i hugo_0.14_amd64.deb
  ```

2. Run server

  ```bash
    $ hugo server --theme=hyde --buildDrafts
  ```

3. Create Some Content

  Hugo also has the ability to create a skeleton content page:

  ```bash
    $ hugo new about.md
  ```

  A new file is now created in content/ with the following contents:

  ```md
    +++
    date = "2015-01-08T08:36:54-07:00"
    draft = true
    title = "about"

    +++
  ```

  > Notice the date is automatically set to the moment you created the content.

  > Place some content in Markdown format below the +++ in this file. For example:

  To create in the subfolder of content mention the relative path and filename

  ```bash
    $ hugo new post/first.md
  ```

  The new file is located at content/post/first.md
