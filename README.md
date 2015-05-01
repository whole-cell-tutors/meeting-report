For purposes of collaborative editing, a server located at Caltech automatically runs LaTeX after every commit to this repository, and publishes the resulting PDF at the following location:

<p align="center">
  http://whole-cell-tutors.github.io/meeting-report/
</p>

You can keep a browser window open on that page, and when a new version is generated, the top of that page will turn red to notify you.  Click on the "reload" button to refresh the PDF.  Note that there is a delay of roughly 10&ndash;15 seconds between the time a commit is received by GitHub and the time the document is refreshed.

The auto-generated preview is useful if you want to edit files online (see below).  If you prefer to edit the files on your local computer in your favorite editor, you do not need to watch the auto-generated preview, since you can use your normal previewing tools and see the same results (and faster).


## Notification of changes

You will want to be notified when changes have been made to the master repository, especially if you are editing in your local editor.  In order to notify everyone when changes have been made, we have set up a mailing list that receives auto-generated email for every commit to the respository:

<p align="center">
  https://groups.google.com/forum/#!forum/whole-cell-report-github
</p>


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

You will need to `git clone` the repository, push your changes back to the repository, regularly check for updates to the repository and `git pull` updates when needed.  If this is unfamiliar, you may want to download one of the following desktop git clients, which provide nice GUI interfaces for these tasks and monitor the repository for remote changes.

* [Windows GitHub client](https://windows.github.com)
* [Mac GitHub  client](https://mac.github.com)
* Linux users may want to look at the 3rd-party git clients [listed here](http://git-scm.com/download/gui/linux)

To learn how to use git, here are two good resources: 

* [https://try.github.io](https://try.github.io)
* [http://git-scm.com](http://git-scm.com)


## Conventions used in the LaTeX files

**Line wrapping**: The LaTeX file uses "soft" line wrapping: instead of using a hard newline to end each text line at some fixed column (e.g., 78 columns), there are no end-of-line newlines, and people's editing environments are assumed to soft-wrap lines at whatever column individual people prefer.  Newlines are only used to separate paragraphs.  (Specifically, two newlines are used to separate paragraphs.)

If you edit files on your local computer, you will probably want to change your git configuration to use *word-oriented* diffs instead of line-oriented diffs.  Tips for doing this are described in a separate section below.

**Tabs**: please use spaces instead of tabs to indicate indentation.  This is necessary because different people configure their editors to have tabs equal a different number of spaces, and if tabs and spaces are mixed (which *invariably* happens), then indentation becomes inconsistent and confusing.


## Setting up word-oriented diffs
