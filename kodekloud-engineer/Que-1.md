useradd is a command in Linux that is used to add user accounts to your system

It is just a symbolic link to adduser command in Linux and the difference between both of them is that useradd is a native binary compiled with the system whereas adduser is a Perl script that uses useradd binary in the background. It makes changes to the following files:

/etc/passwd
/etc/shadow
/etc/group
/etc/gshadow
creates a directory for new user in /home

Syntax for useradd

useradd [options] [User_name]

Options:

  -d,  home directory of the new account
  -e,  expiration date of the new account
  -g,  name or ID of the primary group of the new account
  -G, --groups GROUPS           list of supplementary groups of the new
                                account
  -m, --create-home             create the user's home directory
  -M, --no-create-home          do not create the user's home directory
  -N, --no-user-group           do not create a group with the same name as
                                the user
  -o, --non-unique              allow to create users with duplicate
                                (non-unique) UID
  -p, --password PASSWORD       encrypted password of the new account
  -s, --shell SHELL             login shell of the new account
  -u, --uid UID                 user ID of the new account
  -U, --user-group              create a group with the same name as the user
  -Z, --selinux-user SEUSER     use a specific SEUSER for the SELinux user mapping