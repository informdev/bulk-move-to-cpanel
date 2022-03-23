Your usage may vary. I'm mostly saving this for myself for future use/reference.

On "bulk create cPanel accounts"

Create the file:

nano cpanel_mass_account.sh then input the script inside the above file.

Then run the following:

touch cpanel_mass_account.sh; chmod +x cpanel_mass_account.sh; tee -a cpanel_mass_account.sh

You also need to create a file named something like list.txt and set your perimeters for each account:

TheDomain.com DESIRED_USERNAME DESIRED_PASSWORD
TheDomain.com DESIRED_USERNAME DESIRED_PASSWORD
TheDomain.com DESIRED_USERNAME DESIRED_PASSWORD

etc... Alternatively, you can just input the domain and the script will automatically create usernames and passwords for each one.

Then run the script:

./cpanel_mass_account.sh

It will ask you what file you want to use for loading the accounts (the list.txt you just made), simply put it there.
