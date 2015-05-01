For purposes of collaborative editing, a server located at Caltech automatically runs LaTeX after every commit to this repository, and publishes the resulting PDF at the following location:

<center>
  http://whole-cell-tutors.github.io/meeting-report/
</center>

You can keep a browser window open on this page, and when a new version is generated, the top of the page will turn red to notify you.  Click on the "reload" button to refresh the PDF.  Note that there is a delay of roughly 10&ndash;15 seconds between the time a commit is received by GitHub and the time the document is refreshed.

The preview at the location above is useful if you want to edit files online (see below).  If you prefer to clone the repository and edit the document on your local computer in your favorite editor, you do not need to watch the auto-generated preview, since you can use your normal previewing tools and see the same results (and faster).


## Notification of changes

If you are editing in your local editor, you will want to be notified when changes have been committed to the master repository.  In order to notify people when changes have been made, we have set up a mailing list which receives every commit message to the respository.  You can subscribe to this mailing list here:

  https://groups.google.com/forum/#!forum/whole-cell-report-github


## Options for editing this file

The purpose of this repository and auto-generation system is to offer authors the option to use online editing or local editing, as they wish.  Here are some tips for using either approach.


### If you want to edit directly in your browser

GitHub's online editor does not have very many features, but it is serviceable and very easy to use.  Click on a file name in this repository above.  GitHub will present an editing interface.  Look near the top of the file for the pencil icon,

![github-edit-buttons](https://github.com/mhucka/vireo/raw/master/.readme/github-edit-buttons.png)

and click on it.  Before going further, you will want to change the editor settings.  Look again in the same upper right hand area for the new set of buttons:

![github-edit-buttons](https://github.com/mhucka/vireo/raw/master/.readme/github-nowrap.png)

Do 3 things: (1) click the "nowrap" button and select "Soft wrap" from the pop-up menu, (2) click the "spaces" button and select "Tabs" from the menu, and finally, (3) click the "2" and change the indent size to "8".

![github-edit-buttons](https://github.com/mhucka/vireo/raw/master/.readme/github-soft-wrap.png)

(Sorry, there's no way to set defaults for GitHub's editor, so you have to repeat the procedure every time you edit a file.)


### If you want to edit in a desktop editor

You will need to git clone the repository, push your changes back to the repository, regularly check for updates to the repository and git pull updates when needed.  If this is unfamiliar, you may want to download one of the following desktop git clients, which provide nice GUI interfaces for these tasks and monitor the repository for remote changes.

* [Windows GitHub client](https://windows.github.com)
* [Mac GitHub  client](https://mac.github.com)
* Linux users may want to look at the 3rd-party git clients [listed here](http://git-scm.com/download/gui/linux)

To learn how to use git, here are two good resources: 

* [https://try.github.io](https://try.github.io)
* [http://git-scm.com](http://git-scm.com)




## Conventions used in the LaTeX file

**Line wrapping**: The LaTeX file uses "soft" line wrapping: instead of using a hard newline to end each text line at some fixed column (e.g., 78 columns), people's editing environments are assumed to soft-wrap lines at whatever column individual people prefer.  Newlines are only used to separate paragraphs.  (Specifically, two newlines are used to separate paragraphs.)

With the soft-wrapping convention, if you edit files on your local computer, you will want to change your git configuration to use word-oriented diffs instead of line-oriented diffs.  Tips for doing this are described in a separate section below.

**Tabs**: please use spaces instead of tabs to indicate indentation.  This is necessary because not everyone may uses the same convention for how many spaces equal a tab, and if tags and spaces are mixed (which invariably happens), then indentation becomes inconsistent and confusing.


## Setting up word-oriented diffs
