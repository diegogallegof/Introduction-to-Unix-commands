# Introduction-to-Unix-commands

**Source** <https://kb.iu.edu/d/afsk>

@diegogallegof

Following is a very brief introduction to some useful Unix commands, including examples of how to use each command. For more extensive information about any of these commands, use the `man` command as described below. Sources for more information appear at the end of this document.

On this page:


* [cal](#cal)
* [cat](#cat)
* [cd](#cd)
* [chmod](#chmod)
* [cp](#cp)
* [date](#date)
* [df](#df)
* [du](#du)
* [find](#find)
* [ifconfig](#ifconfig)
* [jobs](#jobs)
* [kill](#kill)
* [less and more](#less-and-more)
* [lpr and lp](#lpr-and-lp)
* [ls](#ls)
* [man](#man)
* [mkdir](#mkdir)
* [mv](#mv)
* [ps](#ps)
* [pwd](#pwd)
* [rm](#rm)
* [rmdir](#rmdir)
* [set](#set)
* [vi](#vi)
* [w and who](#w-and-who)

## cal

This command will print a calendar for a specified month and/or year.

To show this month's calendar, enter:

`cal`

To show a twelve-month calendar for 2008, enter:

`cal 2008`

To show a calendar for just the month of June 1970, enter:

`cal 6 1970`

## cat

This command outputs the contents of a text file. You can use it to read brief files or to concatenate files together.

To append file1 onto the end of file2, enter:

`cat file1 >> file2`

To view the contents of a file named myfile, enter:

`cat myfile`

Because cat displays text without pausing, its output may quickly scroll off your screen. Use the [less](#less-and-more) command (described below) or an editor for reading longer text files.

## cd

This command changes your current directory location. By default, your Unix login session begins in your home directory.

To switch to a subdirectory (of the current directory) named myfiles, enter:

`cd myfiles`

To switch to a directory named **/home/dvader/empire_docs**, enter:


``` cd /home/dvader/empire_docs ```

To move to the parent directory of the current directory, enter:

`cd ..`

To move to the root directory, enter:

`cd /`

To return to your home directory, enter:

`cd`

## chmod

This command changes the permission information associated with a file. Every file (including directories, which Unix treats as files) on a Unix system is stored with records indicating who has permission to read, write, or execute the file, abbreviated as r, w, and x. These permissions are broken down for three categories of user: first, the owner of the file; second, a [group](#group) with which both the user and the file may be associated; and third, all other users. These categories are abbreviated as u for owner (or user), g for group, and o for other.

To allow yourself to execute a file that you own named `myfile`, enter:

`chmod u+x myfile`

To allow anyone who has access to the directory in which `myfile` is stored to read or execute `myfile`, enter:

`chmod o+rx myfile`

You can view the permission settings of a file using the ls command, described below.

* **Note:**
Be careful with the `chmod` command. If you tamper with the directory permissions of your home directory, for example, you could lock yourself out or allow others unrestricted access to your account and its contents.

## cp

## date

## df

## du

## find

## ifconfig

## jobs

## kill

## less and more

## lpr and lp

## ls

## man

## mkdir

## mv

## ps

## pwd

## rm

## rmdir

## set

## vi

## w and who
