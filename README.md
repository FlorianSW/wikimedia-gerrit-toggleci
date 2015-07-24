# Toggle CI for Wikimedia Gerrit
Based on the Hide CI code used in [OpenStack's Gerrit](https://git.openstack.org/cgit/openstack-infra/system-config/tree/modules/openstack_project/files/gerrit/hideci.js). For the use
with Wikimedia's Gerrit installation, I changed the necessary lines.

# Installation
The script is ready for use in Google Chrome as a user script, or an unpacked extension (turn developer mode on). It *should*
be possible to use this script in an userscript management addon for Chrome or any other browser, too.

# What does the script do?
After the installation is finished, the script will be triggered on all URL's matching _https://gerrit.wikimedia.org/r/#/c/*_. It will
parse the comments added by *jenkins-bot* (the CI account for Wikimedia's CI infrastructure) and adds the very latest tests to the top,
at the right side of the reviewer list. There is also an option to hide all comments from jenkins-bot to make the comments list
much more readable (if you don't need to scroll through all test comments).

