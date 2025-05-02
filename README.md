
#echo "deb [trusted=yes] https://sarojamkatel.github.io/yankp-deb/repo ./" | sudo tee /etc/apt/sources.list.d/yankp.list

# what it does:

   # This adds a new APT source to your system by creating a file named yankp.list in /etc/apt/sources.list.d/.

  #  The line inside it tells apt:

    #    deb: This is a Debian package repository.

   #     [trusted=yes]: Trust this source even though it's not signed with a GPG key (ok for personal/testing repos).

  #      https://sarojamkatel.github.io/yankp-deb/repo: This is the URL of the  APT repository (hosted on GitHub Pages).

 #       ./: Use the packages found in that directory without looking for a specific release or distribution name.

# After this step, your system knows where to look for the yankp package.


echo "deb [trusted=yes] https://sarojamkatel.github.io/yankp-deb/repo ./" | sudo tee /etc/apt/sources.list.d/yankp.list
sudo apt update
sudo apt install yankp

