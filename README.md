# AWeber Email Templates

This is a repository of the templates AWeber offers our customers through the message editor. The purpose of this is to:

* Maintain a history of improvements and changes to the templates to ensure we are using a consistent email layout and quality
* Automate the email creation workflow to speed email development and enable stronger innovation in the inbox

## Requirements

* [Node](https://nodejs.org/en/) (>= 4.2.4)
* [npm](http://blog.npmjs.org/post/85484771375/how-to-install-npm) (>= 3.10.6)
* [Foundation for Email - SASS version](http://foundation.zurb.com/emails/docs/sass-guide.html) to make it easy to scaffold templates. Run `sudo npm install --global foundation-cli` in terminal to install this globally.

## Setup

**1.** Clone this repo:

    $ git clone git@github.aweber.io:control-panel/aw-email-templates.git

**2.** Install Foundation for Emails to make it super simple to scaffold new templates.

    $ sudo npm install --global foundation-cli

**3.** Install your dependencies:

    $ sudo npm install

## Developing an Email

### Starting up the Server and Editing the First Template

To start up a local server:

    $ npm start

Once the server is running, it will open a browser window showing you an email at **localhost:3001**. That source for that email lives in `src/index.html`.

While the server is running, any changes you make to your html templates and partials, or SASS stylesheets and partials will automatically update the live view.

### Adding a New Template

The simplest way to add a new template is to duplicate `src/index.html`, rename it, and change the subject line at the top of the template. The new template will then be available at **localhost:3001/YOUR-FILE-NAME**.

💌
