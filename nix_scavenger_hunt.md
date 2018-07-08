# *nix Scavenger Hunt

Complete the following challenges using the command-line interface on your favorite
Unix or Linux operating system. You are welcome and encouraged to consult any
additional documentation online or in books.

Please add your answers/responses/text pastes to the document after each prompt.

Note: For some of the challenges you will need to reference files included with
this repository, so you will need to fork the repo into your own Github account
and then clone it to your development environment.

## The Challenges

### Navigating the Filesystem

* Use the `pwd` command to find your "path to working directory"--your current location in the filesystem of your devbox.
*Paste the output of the `pwd` command here:*

```
/Users/DEREK
```

* Discover more about this filesystem. Use `ls` (the "list" command)to see what is in this directory. *What directories and files do you see when you run `ls`?*

```
I see the list of folders in my current directory.

Applications	Documents	Library		Music		Public
Desktop		Downloads	Movies		Pictures
```

* You can use *options* to modify how a command runs. Try using `ls -alh` to see the contents of your current directory. *How are the results different when you use the `-alh` options?*

```
total 64
drwxr-xr-x+  22 DEREK  staff   748B Jul  4 10:33 .
drwxr-xr-x    6 root   admin   204B Oct 29  2016 ..
-r--------    1 DEREK  staff     7B Oct 29  2016 .CFUserTextEncoding
-rw-r--r--@   1 DEREK  staff    16K Jun  2 19:43 .DS_Store
drwx------  157 DEREK  staff   5.2K Jun 29 18:34 .Trash
drwxr-xr-x   15 DEREK  staff   510B Jun  9 12:27 .atom
-rw-------    1 DEREK  staff   186B Jul  3 16:22 .bash_history
drwx------   19 DEREK  staff   646B Jul  4 10:44 .bash_sessions
drwxr-xr-x    3 DEREK  staff   102B Oct  7  2016 .config
drwx------    3 DEREK  staff   102B Jun 10  2016 .cups
-rw-r--r--    1 DEREK  staff   186B Jul  4 10:33 .gitconfig
drwxr-xr-x    3 DEREK  staff   102B Oct  2  2016 .openvr
drwxr-xr-x    3 DEREK  staff   102B Jan 14  2017 .oracle_jre_usage
drwx------    4 DEREK  staff   136B Dec  2  2015 Applications
drwx------+  45 DEREK  staff   1.5K Jul  3 22:43 Desktop
drwx------+  54 DEREK  staff   1.8K May  2 16:52 Documents
drwx------+  26 DEREK  staff   884B Jul  2 18:02 Downloads
drwx------@  65 DEREK  staff   2.2K Jul  3 15:29 Library
drwx------+   3 DEREK  staff   102B Nov  1  2014 Movies
drwx------+   9 DEREK  staff   306B Jun 29 12:15 Music
drwx------+  28 DEREK  staff   952B Jul  2 18:55 Pictures
drwxr-xr-x+   5 DEREK  staff   170B Nov  1  2014 Public
```

* The `man` ("manual") command tells you more about how any given command works. Run `man` to see instructions about how to use `man`. Then use `man` to learn what the `a`, `l`, and `h` options mean when used with the `ls` command. *Write down what those options do?*

```
    -a      What manual page do you want?
    -h      Print a help message and exit.
    -l      Activate 'local' mode. Format and display local manual files instead of searching through the system's manual collection.
```

* Commands can also take *arguments*, which are usually the names of files or locations that you want the command to work with. Try running `ls /` to see what files are in the *root* directory of the filesystem. *What files and directories do you see listed?*

```
Applications			etc
Library				home
Network				installer.failurerequests
System				net
Users				private
Volumes				sbin
bin				tmp
cores				usr
dev				var
```

* A Unix filesystem has a few special shortcuts to refer to specific locations. `/` indicates the *root* of the filesystem, meaning the top-most directory in the filesystem hierarchy. Use the `cd` ("change directory") command to move to the root directory. (Hint: Use `man` to look up the `cd` command if you have any issues) *Then run `pwd` and paste the output here:*

```
/
Dereks-MacBook-Pro:/ DEREK$
```

* Another special shortcut in Unix is the `~` location. This indicates the *user root* directory, meaning the top-most directory in the hierarchy that comes below your user account. Use `cd` to move to `~`. *Run `pwd` and paste the response here:*

```
/Users/DEREK
```

* Change directory into the `challenge_files` directory. Use `ls` to find only the files with a `.demo` pattern. *How many files do you find?*

```
3 files named with .demo

01				Hillard-Ziemann.user
2015_special_stuff.demo		Isadora-Leffler.user
Afton-Jast.user			Jaxen-Gleichner.user
Aimee-Maggio.user		Jayme-Rodriguez.user
Alfonso-Gottlieb.user		Jenni-O'Connell.user
Allen-Kemmer.user		Johny-Borer.user
Almina-Cormier.user		Kassandra-Barrows.user
Alta-Lemke.user			Keely-Hilpert.user
Amina-McGlynn.user		Kenyatta-Hickle.user
Anabel-Hammes.user		Kiana-Kulas.user
Ancel-Conn.user			Kirstin-Hoppe.user
Anjali-Halvorson.user		Kwame-Schmitt.user
Ardath-Kuvalis.user		Ladonna-Lueilwitz.user
Avah-Dickinson.user		Lala-Will.user
Ayaan-Stiedemann.user		Leia-Hudson.user
Aylin-Grant.user		Leia-Ziemann.user
Bedford-Sipes.user		Lillard-Purdy.user
Benita-King.user		Lilly-Kohler.user
Benito-Stoltenberg.user		Lissie-Strosin.user
Beverlee-Moen.user		Mannie-Ritchie.user
Brad-Thiel.user			Masako-Lind.user
Brayan-Douglas.user		Melisa-Yundt.user
Bria-Satterfield.user		Michelina-Kuphal.user
Bridgette-Reichel.user		Minnie-Jacobi.user
Britt-Erdman.user		Murdock-Leffler.user
Britta-Hammes.user		Mychal-Corkery.user
Bryant-Kuhic.user		Nakita-Nader.user
Bryton-Aufderhar.user		Nayely-Dare.user
Caitlin-Grady.user		Nicholas-Strosin.user
Carroll-Hartmann.user		Niles-Runte.user
Claudie-McClure.user		Nina-Sporer.user
Clemente-Haley.user		Noreta-Steuber.user
Cleo-VonRueden.user		Ovid-Bogan.user
Codie-Romaguera.user		Randell-Sauer.user
Cooper-Reynolds.user		Remy-Renner.user
Corrie-Bogisich.user		Ronna-Hermann.user
Dannielle-Green.user		Rosalind-Wisozk.user
Deedee-Jacobson.user		Rosena-Simonis.user
Desiree-Marks.user		Sandie-Balistreri.user
Deven-Rutherford.user		Sharen-Hansen.user
Doyle-Jones.user		Sherrill-Russel.user
Dustyn-O'Connell.user		Sherwin-Kovacek.user
Elza-Mraz.user			Sherwood-Rath.user
Emory-Crona.user		Shyheim-Murazik.user
Erin-Walker.user		Siobhan-Kirlin.user
Estela-Schultz.user		Tomas-Kutch.user
Fernanda-Tromp.user		cloaked-wookie.demo
Fletcher-Rice.user		credit_cards.txt
Fred-Ryan.user			credit_cards2.txt
Genie-Abshire.user		scooter-double-mamba.demo
Grace-Tromp.user		serial-numbers
Grant-Cronin.user		test2
Hali-Roob.user			tmp
Harland-Schoen.user		wow
Harrell-Quitzon.user
```

* Use the `cd` command to move "up" one directory. *Where are you in the filesystem now?* I am one level up in my current directory.

```
Dereks-MacBook-Pro:wats1030-intro-to-unix DEREK$
```

* Press the up arrow on your keyboard. *What just happened?* I see my last typed command.

```
Dereks-MacBook-Pro:wats1030-intro-to-unix DEREK$ cd ..
```

* Press the up arrow a few more times. *What do you see?* I see my last few previous commands.

```
Dereks-MacBook-Pro:wats1030-intro-to-unix DEREK$ cd wats1030-intro-to-unix/
```

* Run the `history` command. *What do you see?*

```
I see Bash's log of commands I have typed.
1  git config --global user.name "Dere Benak"
2  git config --global user.email "benakderek@seattleu.edu"
3  cat wats3010-css/.git/config
4  cat wats3010-css/.git/config
5  :~Documents
6  w
7  ifconfig
8  cp m
9  pwd
10  ls
11  ls -alh
12  man -als
13  man -a ls
14  man a
15  man1
16  mana
17  als
18  a ls
19  a-ls
20  man a-ls
21  man a
22  man-a
23  man ls
24  ls /
25  man ls
26  man -a
27  h
28  man -a
29  -h
30  man -a
31  l
32  man -a
33  -l
34  man -a
35  man -h
36  man ls -a
37  man ls -h
38  man ls -l
39  man -l ls
40  man -a
41  man -h
42  man -l
43  man -l
44  ls /
45  man ls -h
46  man -a
47  cd
48  ls /
49  cd
50  pwd
51  man -l
52  ls /
53  cd
54  cd /
55  / cd
56  man
57  cd
58  man
59  -cd
60  man man
61  ls /
62  cd /
63  pwd
64  pwd
65  -h
66  man -h
67  cd
68  cd /
69  cd/
70  man cd
71  pwd
72  cd ~
73  cd [~]
74  cd ~
75  pwd
76  cd /
77  pwd
78  pwd
79  cd challenge_files
80  cd /WATS_3030/Week_2/wats1030-intro-to-unix/challenge_files
81  cd /Macintosh_HD/Users/Derek/Desktop/wats1030-intro-to-unix
82  cd /
83  cd ~
84  cd /
85  pwd
86  cd ~
87  pwd
88  cd /
89  pwd
90  cd ~
91  pwd
92  cd Derek$
93  cd WATS_3030
94  cd /home/Derek/Desktop/WATS_3030
95  ls
96  cd Desktop/
97  ls
98  cd
99  Desktop/WATS 3030/
100  CD Desktop/
101  ls
102  cd Desktop/
103  ls
104  cd Desktop/WATS 3030/
105  cd Desktop/
106  cd
107  ls
108  cd Desktop/
109  cd WATS_3030/
110  ls
111  cd week_2/
112  cd Week 2/
113  cd Week_2/
114  cd wats1030-intro-to-unix/
115  cd challenge_files/
116  ls
117  cd ..
118  history
```

### Observing the System

* Discover what account you are logged into using the `whoami` command. *What username are you currently using?*

```
DEREK
```

* Discover who else is on your system with the `who` command. *Are any other users using your system? If so, list them here:*

```
DEREK    console  Jun  5 14:59
DEREK    ttys000  Jul  4 12:00
```

* How long has your system been running? Use `uptime` to see, and *paste the result here:*

```
12:48  up 28 days, 21:55, 2 users, load averages: 2.67 2.22 1.99
```

* Run `ps aux` and review the results. (Hint: Use `man` to learn more about the `ps` command and options.) *How do you interpret what you see here?*
This showed all of your active processes that have controlling terminals on my computer.

```
USER               PID  %CPU %MEM      VSZ    RSS   TT  STAT STARTED      TIME COMMAND
DEREK            21943   5.1  2.7  3624344 230436   ??  S     3:30PM  11:57.76 /Applications/Go
DEREK            21927   4.4  2.4  3774800 198728   ??  S     3:30PM  14:38.95 /Applications/Go
DEREK            21944   2.1  1.5  3541484 122204   ??  S     3:30PM   8:37.83 /Applications/Go
DEREK            22987   2.0  1.5  3172916 128996   ??  S    10:46AM   3:57.50 /Applications/Sp
_coreaudiod        150   2.0  0.1  2520048   4328   ??  Ss    5Jun18 193:49.77 /usr/sbin/coreau
_windowserver      149   1.4  1.1  4208712  91148   ??  Ss    5Jun18 443:35.97 /System/Library/
DEREK            21959   1.4  0.5  2721604  43184   ??  S     3:32PM   1:19.07 /Applications/Ut
DEREK            23734   1.0  2.1  4016144 173048   ??  S    12:01PM   1:47.55 /Applications/At
DEREK            21467   0.5  0.7 18464608  56844   ??  S    Mon03PM  10:30.86 /Applications/Go
DEREK            21928   0.5  2.0  3674064 164692   ??  S     3:30PM   4:10.76 /Applications/Go
DEREK            23647   0.5  1.0  3453520  84888   ??  S    11:54AM   0:26.03 /Applications/Go
DEREK            22996   0.5  1.2  3799924 100576   ??  S    10:46AM   1:32.43 /Applications/Sp
_hidd              121   0.5  0.0  2518604   3844   ??  Ss    5Jun18 119:04.50 /usr/libexec/hid
DEREK            22571   0.3  0.6  3507784  46440   ??  S    10:28AM   0:13.43 /Applications/Go
DEREK            15377   0.2  3.9  3816752 327860   ??  S    24Jun18 161:02.62 /Applications/Go
DEREK            21929   0.2  0.8  3425396  65532   ??  S     3:30PM   0:14.90 /Applications/Go
DEREK            21305   0.1  0.0  2515560   3464   ??  S    Mon11AM   0:05.76 /System/Library/
DEREK            23862   0.1  1.7  3665040 141636   ??  S    12:12PM   0:18.34 /Applications/Go
DEREK            18433   0.1  0.2  2913860  17792   ??  Ss   Wed07PM   0:26.71 /System/Library/
DEREK              462   0.1  0.0  2567524   4108   ??  S     5Jun18   1:32.86 /System/Library/
DEREK            17666   0.1  1.3  3751616 109848   ??  S    Wed04PM   9:37.65 /Applications/Go
DEREK            22970   0.1  1.4  3540400 118060   ??  S    10:45AM   0:39.64 /Applications/Go
root             23124   0.0  0.0  2461744    384   ??  SNs  11:08AM   0:00.01 /usr/libexec/per
DEREK            22992   0.0  0.0  2516612   2364   ??  Ss   10:46AM   0:00.04 /System/Library/
DEREK            22991   0.0  0.1  2866296  12536   ??  S    10:46AM   0:00.76 /Applications/Sp
DEREK            22990   0.0  0.1  2742868   9048   ??  S    10:46AM   0:00.15 /Applications/Sp
_spotlight       22856   0.0  0.1  2497892   5088   ??  S    10:40AM   0:00.13 /System/Library/
DEREK            22614   0.0  0.0  2533080   2592   ??  S<   10:33AM   0:00.04 /Applications/Gi
DEREK            22584   0.0  0.6  3464712  47940   ??  S    10:33AM   0:09.41 /Applications/Gi
DEREK            22578   0.0  0.7  3628180  59496   ??  S    10:32AM   0:21.71 /Applications/Gi
DEREK            22573   0.0  0.5  4108628  39592   ??  S    10:30AM   0:03.33 /Applications/Go
DEREK            22557   0.0  0.6  3547620  48068   ??  S    10:23AM   0:24.59 /Applications/Go
DEREK            22555   0.0  0.6  3551496  52684   ??  S    10:23AM   0:18.88 /Applications/Go
_netbios         22459   0.0  0.0  2517844   2560   ??  SNs  10:18AM   0:00.12 /usr/sbin/netbio
DEREK            22082   0.0  0.5  3623244  45380   ??  S     3:59PM   0:05.85 /Applications/Go
DEREK            21977   0.0  0.5  3366424  38576   ??  S     3:32PM   0:02.21 /Applications/Go
_iconservices    21968   0.0  0.0  2520860   3664   ??  Ss    3:32PM   0:00.10 /System/Library/
root             21961   0.0  0.0  2491512   2112   ??  Ss    3:32PM   0:00.03 /System/Library/
DEREK            21955   0.0  0.4  3361992  29444   ??  S     3:31PM   0:02.47 /Applications/Go
DEREK            21954   0.0  0.7  3386280  58140   ??  S     3:31PM   0:06.73 /Applications/Go
DEREK            21953   0.0  0.3  3361860  27680   ??  S     3:31PM   0:02.53 /Applications/Go
DEREK            21952   0.0  0.5  3400472  41252   ??  S     3:31PM   0:10.66 /Applications/Go
DEREK            21951   0.0  0.7  3389764  58004   ??  S     3:30PM   0:22.26 /Applications/Go
DEREK            21948   0.0  0.4  3359812  30272   ??  S     3:30PM   0:01.12 /Applications/Go
DEREK            21946   0.0  1.1  3465204  88580   ??  S     3:30PM   0:34.80 /Applications/Go
DEREK            21942   0.0  0.9  3412888  73160   ??  S     3:30PM   0:14.51 /Applications/Go
DEREK            21941   0.0  0.4  3374028  32584   ??  S     3:30PM   0:08.09 /Applications/Go
DEREK            21936   0.0  0.5  3369352  40616   ??  S     3:30PM   0:03.49 /Applications/Go
DEREK            21930   0.0  0.4  3364708  31816   ??  S     3:30PM   0:04.21 /Applications/Go
root             21894   0.0  0.1  2542032   4196   ??  Ss    3:11PM   0:00.12 /usr/libexec/fin
DEREK            21691   0.0  0.5  3624368  45236   ??  S    Mon06PM   0:05.17 /Applications/Go
DEREK            21690   0.0  0.6  3637852  46872   ??  S    Mon06PM   0:09.18 /Applications/Go
DEREK            21687   0.0  0.5  3625492  44812   ??  S    Mon06PM   0:08.74 /Applications/Go
DEREK            21488   0.0  0.0  2510524   2736   ??  Ss   Mon04PM   0:00.06 /System/Library/
DEREK            21483   0.0  0.0  2480948   1328   ??  S    Mon04PM   0:00.02 /System/Library/
root             21482   0.0  0.0  2479592   1612   ??  Ss   Mon04PM   0:00.01 /System/Library/
DEREK            21471   0.0  0.5  3512540  40972   ??  S    Mon04PM   0:03.76 /Applications/Go
DEREK            21469   0.0  0.5  3954168  38760   ??  S    Mon04PM   0:06.07 /Applications/Go
DEREK            21431   0.0  0.4  3398360  36924   ??  S    Mon03PM   0:13.16 /Applications/Go
DEREK            21394   0.0  0.0  2515556   1792   ??  S    Mon03PM   0:00.04 /System/Library/
DEREK            21303   0.0  0.1  2541600   4940   ??  S    Mon11AM   0:00.09 /System/Library/
_nsurlstoraged   21100   0.0  0.0  2498688   2604   ??  Ss   Sun07PM   0:00.07 /usr/libexec/nsu
DEREK            21047   0.0  1.1  3689432  92756   ??  S    Sun07PM   4:56.64 /Applications/Go
DEREK            20652   0.0  0.0  2545480   4036   ??  S    Sun12PM   0:00.24 /System/Library/
DEREK            20362   0.0  0.1  2622612   9464   ??  S    Sat08PM   0:24.54 /usr/libexec/Saf
DEREK            20331   0.0  0.0  2515312   2456   ??  S    Sat04PM   0:00.16 /System/Library/
DEREK            20297   0.0  0.0  2542464   3640   ??  S    Sat04PM   0:00.54 /System/Library/
DEREK            20295   0.0  0.0  2514612   2680   ??  S    Sat04PM   0:00.08 /System/Library/
DEREK            20274   0.0  0.0  2516832   3364   ??  Ss   Sat04PM   0:00.46 /Library/Framewo
DEREK            20236   0.0  0.2  2729584  17304   ??  Ss   Sat04PM   5:46.80 /System/Library/
root             20234   0.0  0.0  2482224    384   ??  SNs  Sat04PM   0:00.03 /usr/libexec/per
root             20135   0.0  0.0  2545468   2572   ??  Ss   Sat02PM   0:00.10 /System/Library/
root             20133   0.0  0.0  2506580   1944   ??  Ss   Sat02PM   0:00.03 /usr/libexec/smd
DEREK            20132   0.0  0.0  2515312   2140   ??  S    Sat02PM   0:00.05 /usr/libexec/log
DEREK            20077   0.0  0.2  2642216  12964   ??  S    Sat02PM   0:28.07 /System/Library/
DEREK            20075   0.0  0.0  2506020   2240   ??  S    Sat02PM   0:00.06 /System/Library/
DEREK            20074   0.0  0.0  2542552   3988   ??  S    Sat02PM   0:00.86 /System/Library/
DEREK            20016   0.0  0.5  3512104  40168   ??  S    Sat11AM   0:05.24 /Applications/Go
DEREK            20003   0.0  0.0  2515884   2240   ??  S    Sat11AM   0:00.12 /System/Library/
root             19987   0.0  0.0  2537436   3316   ??  Ss   Sat11AM   0:00.18 /usr/libexec/neh
DEREK            19961   0.0  0.0  2515184   2544   ??  S    Sat09AM   0:00.14 /System/Library/
DEREK            19941   0.0  0.1  2627404  10424   ??  S    Sat09AM   0:06.11 /System/Library/
root             19916   0.0  0.0  2541212   3056   ??  Ss   Sat09AM   0:00.97 /usr/libexec/san
DEREK            19910   0.0  0.1  2544860   5628   ??  S    Sat09AM   0:03.17 /System/Library/
DEREK            19908   0.0  0.0  2515796   3280   ??  S    Sat09AM   0:00.15 /System/Library/
root             19906   0.0  0.0  2542376   3160   ??  Ss   Sat09AM   0:00.26 /usr/libexec/wif
DEREK            19904   0.0  0.1  2547304  10832   ??  S    Sat09AM   0:01.14 /System/Library/
DEREK            19903   0.0  0.1  2545112   5216   ??  S    Sat09AM   0:00.73 /System/Library/
DEREK            19902   0.0  0.1  2542920   5064   ??  S    Sat09AM   0:02.47 /usr/libexec/WiF
DEREK            19901   0.0  0.1  2547324   9296   ??  S    Sat09AM   0:00.90 /System/Library/
root             19890   0.0  0.0  2498652   1724   ??  Ss   Sat09AM   0:00.03 /usr/sbin/aslman
_ctkd            19885   0.0  0.0  2499024   1704   ??  Ss   Sat12AM   0:00.05 /System/Library/
DEREK            19884   0.0  0.0  2516448   1972   ??  S    Sat12AM   0:00.06 /System/Library/
DEREK            19883   0.0  0.0  2514780   1732   ??  S    Sat12AM   0:00.06 /System/Library/
root             19882   0.0  0.0  2541948   3408   ??  Ss   Sat12AM   0:00.43 /usr/libexec/sec
root             19881   0.0  0.0  2514780   1636   ??  Ss   Sat12AM   0:00.08 /System/Library/
root             19880   0.0  0.0  2540632   2980   ??  Ss   Sat12AM   0:00.24 /System/Library/
DEREK            19788   0.0  0.0  2540184   2296   ??  S    Fri11PM   0:00.08 /System/Library/
root             19787   0.0  0.0  2515036   1852   ??  Ss   Fri11PM   0:00.29 aslmanager
root             19786   0.0  0.0  2517256   1684   ??  Ss   Fri11PM   0:00.21 /System/Library/
DEREK            19785   0.0  0.0  2539976   2660   ??  S    Fri11PM   0:00.12 /System/Library/
_assetcache      19784   0.0  0.0  2545276   3064   ??  Ss   Fri11PM   0:00.13 /usr/libexec/Ass
DEREK            19783   0.0  0.1  2543940   4408   ??  S    Fri11PM   0:02.15 /usr/libexec/pkd
DEREK            19782   0.0  0.0  2542176   3180   ??  S    Fri11PM   0:00.37 /System/Library/
DEREK            19765   0.0  0.0  2545092   4064   ??  S    Fri11PM   0:01.48 /System/Library/
DEREK            19695   0.0  0.0  2544192   3828   ??  S    Fri10PM   0:00.29 /System/Library/
DEREK            19651   0.0  0.1  2551848   5608   ??  S    Fri09PM   0:05.91 /System/Library/
DEREK            19650   0.0  0.2  2545168  15164   ??  Ss   Fri09PM   0:02.57 /System/Library/
DEREK            19648   0.0  0.0  2516300   2780   ??  S    Fri09PM   0:00.50 /System/Library/
DEREK            19646   0.0  0.1  2554396  10180   ??  S    Fri09PM   0:21.36 /System/Library/
DEREK            19613   0.0  0.1  2642636   5484   ??  S    Fri09PM   0:00.27 /System/Library/
root             19612   0.0  0.1  2541572   4532   ??  Ss   Fri09PM   0:00.81 /System/Library/
DEREK            19611   0.0  0.0  2514688   1724   ??  S    Fri09PM   0:01.25 /System/Library/
DEREK            19610   0.0  0.1  2547072   6720   ??  S    Fri09PM   0:05.44 /System/Library/
root             19609   0.0  0.0  2498568   2300   ??  Ss   Fri09PM   0:00.03 /System/Library/
root             19608   0.0  0.1  2549756   4292   ??  Ss   Fri09PM   0:02.50 /usr/sbin/system
DEREK            19607   0.0  0.0  2515020   1724   ??  S    Fri09PM   0:00.04 /System/Library/
DEREK            19603   0.0  0.1  3593584   4624   ??  S    Fri09PM   0:00.36 /System/Library/
root             19602   0.0  0.0  2548340   3616   ??  Ss   Fri09PM   0:01.65 /usr/libexec/mob
DEREK            19600   0.0  0.1  2541112   4568   ??  S    Fri09PM   0:00.71 /System/Library/
DEREK            19597   0.0  0.0  2515540   2328   ??  S    Fri09PM   0:00.08 /System/Library/
DEREK            19595   0.0  0.1  2550800  11660   ??  S    Fri09PM   0:45.46 /System/Library/
DEREK            19593   0.0  0.1  2545580   5780   ??  Ss   Fri09PM   0:02.95 /System/Library/
DEREK            19592   0.0  0.0  2543508   4184   ??  S    Fri09PM   0:00.33 /usr/libexec/net
_spotlight       19588   0.0  0.0  2542492   2680   ??  S    Fri09PM   0:01.57 /usr/libexec/tru
DEREK            19566   0.0  0.2  2599256  20816   ??  S    Fri08PM   0:10.70 /System/Library/
DEREK            19565   0.0  0.0  2543784   3732   ??  S    Fri08PM   0:03.55 /usr/libexec/sec
DEREK            19563   0.0  0.0  2514732   3316   ??  S    Fri08PM   0:01.87 /System/Library/
DEREK            19562   0.0  0.0  2542500   3712   ??  S    Fri08PM   0:01.42 /System/Library/
DEREK            19561   0.0  0.0  2542148   3692   ??  S    Fri08PM   0:00.91 /usr/libexec/sec
DEREK            19560   0.0  0.2  2606736  17976   ??  S    Fri08PM   0:09.35 /System/Library/
root             19559   0.0  0.1  2541560   6212   ??  Ss   Fri08PM   0:01.16 /System/Library/
DEREK            19115   0.0  0.0  2516424   2596   ??  S    Fri03PM   0:04.71 /Users/DEREK/Lib
DEREK            19102   0.0  0.1  2568836   7984   ??  S    Fri03PM   0:07.33 /Library/Applica
DEREK            19101   0.0  0.5  1048516  39880   ??  S    Fri03PM   2:12.37 /Applications/Mi
DEREK            18824   0.0  0.7  3939732  60952   ??  S    Fri10AM   2:41.52 /Applications/Sl
DEREK            17673   0.0  0.5  3415132  41804   ??  S    Wed04PM   0:06.37 /Applications/Go
DEREK            17667   0.0  0.6  3531008  51248   ??  S    Wed04PM   1:21.30 /Applications/Go
root             17561   0.0  0.0  2517176   1772   ??  Ss   Wed04PM   0:00.26 /usr/libexec/sys
_softwareupdate  17078   0.0  0.0  2542028   3356   ??  Ss   26Jun18   0:02.33 /System/Library/
DEREK            16478   0.0  0.4  3637336  37400   ??  S    25Jun18   1:47.95 /Applications/Sl
DEREK            16473   0.0  0.4  3508428  33864   ??  S    25Jun18   0:15.99 /Applications/Sl
DEREK            16468   0.0  0.2  2828688  12972   ??  S    25Jun18   1:17.09 /Applications/Sl
DEREK            16466   0.0  0.8  3756720  67036   ??  S    25Jun18   8:28.48 /Applications/Sl
DEREK            15449   0.0  0.0  2541592   3056   ??  S    24Jun18   0:02.69 /usr/libexec/vid
DEREK            15448   0.0  0.0  2542396   2940   ??  S    24Jun18   0:00.64 /usr/libexec/swc
DEREK            15405   0.0  0.6  3402612  51848   ??  S    24Jun18   0:45.21 /Applications/Go
DEREK            15394   0.0  0.5  3419688  42528   ??  S    24Jun18   0:07.65 /Applications/Go
DEREK            15389   0.0  1.2  3792608 102340   ??  S    24Jun18   6:00.69 /Applications/Go
DEREK            15384   0.0  0.2  2861716  20424   ??  S    24Jun18   0:23.05 /Applications/Go
DEREK            15381   0.0  0.0  2517224   2160   ??  S    24Jun18   0:00.13 /Applications/Go
_gamecontrollerd 15379   0.0  0.0  2515828   3828   ??  Ss   24Jun18   0:17.72 /usr/libexec/gam
DEREK            15112   0.0  0.1  2568524   4768   ??  S    24Jun18   0:02.49 /System/Library/
DEREK            14834   0.0  0.2  2594764  18896   ??  S    24Jun18   1:20.78 /System/Library/
DEREK            14726   0.0  0.3  2570448  26968   ??  S    23Jun18   1:07.97 /System/Library/
DEREK            14723   0.0  0.2  2572120  17704   ??  S    23Jun18   0:15.25 /System/Library/
root             14660   0.0  0.1  2543488   7068   ??  S    23Jun18   0:06.06 /System/Library/
DEREK            14638   0.0  0.0  2515612   2664   ??  S    23Jun18   0:00.12 /usr/libexec/spi
root             14637   0.0  0.0  2661576   3768   ??  Ss   23Jun18   0:11.31 /usr/sbin/spindu
root             14597   0.0  0.0  2545588   3232   ??  Ss   23Jun18   0:02.93 /usr/libexec/amf
DEREK            14590   0.0  0.2  2553656  18948   ??  Ss   23Jun18   1:57.38 /System/Library/
DEREK            14587   0.0  0.6  2704776  47544   ??  S    23Jun18   0:52.94 /System/Library/
root             14585   0.0  0.0  2518260   2076   ??  Ss   23Jun18   0:01.23 /System/Library/
root             14582   0.0  0.2  2552228  19116   ??  Ss   23Jun18   0:56.85 /usr/libexec/cor
root             14581   0.0  0.1  2544352   5260   ??  Ss   23Jun18   1:14.47 /System/Library/
DEREK            14570   0.0  0.3  2578856  22076   ??  S    23Jun18   0:59.15 /System/Library/
DEREK            14497   0.0  0.1  3600856   7548   ??  Ss   23Jun18   0:11.34 /System/Library/
DEREK            13782   0.0  0.1  2547376   5344   ??  S    22Jun18   0:02.22 /usr/libexec/key
DEREK            13675   0.0  0.1  2542696   5428   ??  S    22Jun18   0:12.29 /usr/libexec/nsu
DEREK             9921   0.0  0.1  2544336   6192   ??  S    16Jun18   0:01.51 /usr/libexec/avc
DEREK             7370   0.0  0.0  2514992   1588   ??  S    13Jun18   0:00.07 /System/Library/
DEREK             3551   0.0  0.1  2564072   6116   ??  S     8Jun18   0:23.88 /System/Library/
root              2123   0.0  0.0  2506356   1736   ??  Ss    7Jun18   0:00.04 /System/Library/
root              2118   0.0  0.0  2555832   3008   ??  Ss    7Jun18   0:04.59 /System/Library/
DEREK             1339   0.0  0.0  2557284   3560   ??  S     6Jun18 164:34.53 /System/Library/
DEREK              898   0.0  0.0  2516124   1544   ??  S     5Jun18   0:00.17 /usr/libexec/USB
DEREK              846   0.0  0.0  2541112   1828   ??  S     5Jun18   0:03.63 /System/Library/
_fpsd              753   0.0  0.0  2477980    536   ??  Ss    5Jun18   0:00.04 /System/Library/
root               698   0.0  0.0  2546432   1888   ??  Ss    5Jun18   0:01.28 /usr/libexec/dpr
root               675   0.0  0.0  2514704    624   ??  Ss    5Jun18   0:00.28 /System/Library/
DEREK              600   0.0  0.1  2558236   4652   ??  S     5Jun18   0:24.49 /System/Library/
root               547   0.0  0.0  2458572     44   ??  S     5Jun18   0:00.05 /System/Library/
DEREK              546   0.0  0.0  2466764    276   ??  S     5Jun18   0:08.53 /System/Library/
_spotlight         541   0.0  0.0  2515040    704   ??  S     5Jun18   0:02.28 /usr/sbin/distno
DEREK              517   0.0  0.1  2566136   4308   ??  S     5Jun18   0:23.19 /System/Library/
DEREK              516   0.0  0.0  2567284   3660   ??  S     5Jun18   0:25.52 /System/Library/
DEREK              509   0.0  0.0  2541232    400   ??  S     5Jun18   0:00.27 /System/Library/
DEREK              496   0.0  0.1  2553904   5800   ??  S     5Jun18   0:29.38 /System/Library/
DEREK              483   0.0  0.1  2538204   4200   ??  S     5Jun18   0:21.38 /Applications/iT
root               482   0.0  0.0  2540256   3836   ??  Ss    5Jun18   0:01.60 /usr/libexec/tas
DEREK              478   0.0  0.0  2545244   3716   ??  S     5Jun18   0:07.37 /System/Library/
DEREK              477   0.0  0.1  2541104   4500   ??  S     5Jun18   0:10.43 /System/Library/
DEREK              476   0.0  0.0  2565364   3504   ??  S     5Jun18   0:26.67 /System/Library/
DEREK              474   0.0  0.1  2568812   5908   ??  S     5Jun18   0:30.69 /System/Library/
DEREK              473   0.0  0.0  2541340   1720   ??  S     5Jun18   0:01.02 /System/Library/
DEREK              472   0.0  0.0  2556872   3076   ??  S     5Jun18   0:32.22 /System/Library/
DEREK              469   0.0  0.1  2552644   7548   ??  S     5Jun18   1:06.98 /usr/libexec/sha
DEREK              468   0.0  0.0  2540148    280   ??  S     5Jun18   0:00.56 /System/Library/
DEREK              464   0.0  0.0  2541192   1864   ??  S     5Jun18   0:00.88 /System/Library/
DEREK              461   0.0  0.2  2800860  18164   ??  S     5Jun18   1:24.69 /System/Library/
DEREK              457   0.0  0.0  2542004   1140   ??  S     5Jun18   0:04.30 /System/Library/
DEREK              440   0.0  0.6  2756804  48244   ??  S     5Jun18   1:05.64 /System/Library/
DEREK              430   0.0  0.1  2564532   4712   ??  Ss    5Jun18   1:01.01 /System/Library/
DEREK              427   0.0  0.0  2540944   3408   ??  Ss    5Jun18   0:10.18 /System/Library/
DEREK              425   0.0  0.0  2559384   2716   ??  S     5Jun18   0:20.55 /System/Library/
DEREK              418   0.0  0.1  2567652   5836   ??  Ss    5Jun18   0:28.91 /System/Library/
DEREK              417   0.0  0.2  2822456  15112   ??  S     5Jun18   4:58.50 /System/Library/
DEREK              414   0.0  0.2  3002672  19660   ??  S     5Jun18   1:08.24 /System/Library/
DEREK              410   0.0  0.1  2575444   6224   ??  S     5Jun18   1:40.81 /System/Library/
DEREK              409   0.0  0.4  2778696  34980   ??  S     5Jun18   2:50.07 /System/Library/
DEREK              408   0.0  0.2  2704704  17744   ??  S     5Jun18   1:38.73 /System/Library/
DEREK              407   0.0  0.3  2814044  21488   ??  S     5Jun18   4:15.29 /System/Library/
DEREK              406   0.0  0.8  4421728  64608   ??  S     5Jun18  13:21.62 /Applications/Me
DEREK              401   0.0  0.3  3784752  28780   ??  S     5Jun18   1:03.75 /Applications/St
DEREK              400   0.0  0.1  2666832   8784   ??  S     5Jun18   6:21.29 /Applications/Ut
DEREK              397   0.0  0.0  2546452   4168   ??  S     5Jun18   0:07.20 /System/Library/
DEREK              393   0.0  0.0  2541168    832   ??  Ss    5Jun18   0:03.33 /System/Library/
root               381   0.0  0.0  2556328   3060   ??  Ss    5Jun18   0:07.81 /System/Library/
DEREK              378   0.0  0.2  3640028  14976   ??  S     5Jun18   0:08.44 /System/Library/
root               377   0.0  0.0  2616500   3132   ??  Ss    5Jun18   0:15.19 /System/Library/
root               376   0.0  0.0  2515500   1364   ??  Ss    5Jun18   0:00.24 /System/Library/
DEREK              371   0.0  0.0  2514504   1284   ??  S     5Jun18   0:00.81 /System/Library/
DEREK              370   0.0  0.2  2543044  13052   ??  S     5Jun18   0:02.17 /System/Library/
DEREK              367   0.0  0.0  2543056   4136   ??  S     5Jun18   0:31.13 /System/Library/
root               366   0.0  0.0  2574560   3708   ??  Ss    5Jun18   0:13.56 /System/Library/
DEREK              362   0.0  0.0  2543940   3208   ??  Ss    5Jun18   0:04.58 /System/Library/
root               359   0.0  0.0  2518924   2584   ??  Ss    5Jun18   0:13.40 /usr/sbin/fileco
DEREK              355   0.0  0.1  2549016   5400   ??  S     5Jun18   0:46.56 /System/Library/
DEREK              354   0.0  0.1  2560692   7800   ??  S     5Jun18   1:15.42 /System/Library/
DEREK              351   0.0  0.1  2548908   5924   ??  S     5Jun18   0:15.78 /System/Library/
DEREK              349   0.0  0.1  2591068   6192   ??  S     5Jun18   0:09.85 /System/Library/
DEREK              348   0.0  0.0  2532016   2316   ??  S     5Jun18   0:02.06 /usr/libexec/pbo
DEREK              344   0.0  0.1  2542880   6112   ??  S     5Jun18   0:12.74 /System/Library/
DEREK              320   0.0  0.3  2569992  25236   ??  S     5Jun18   9:06.96 /System/Library/
DEREK              318   0.0  0.0  2545104   3892   ??  S     5Jun18   0:20.76 /usr/libexec/nsu
DEREK              317   0.0  0.1  2545264   4596   ??  S     5Jun18   0:25.71 /usr/sbin/userno
DEREK              315   0.0  0.0  2543112    208   ??  S     5Jun18   0:00.55 /usr/libexec/lan
DEREK              311   0.0  0.1  2547668   7964   ??  S     5Jun18   5:41.35 /usr/libexec/tru
DEREK              310   0.0  0.1  2548708   4612   ??  S     5Jun18   1:04.99 /usr/libexec/lsd
DEREK              307   0.0  0.0  2516612   3560   ??  S     5Jun18   1:34.57 /usr/sbin/distno
DEREK              305   0.0  0.1  2542396   6152   ??  S     5Jun18   0:36.36 /usr/libexec/Use
root               304   0.0  0.0  2542608    828   ??  Ss    5Jun18   0:00.51 /System/Library/
DEREK              303   0.0  0.0  2522764   3696   ??  S     5Jun18   1:04.85 /usr/sbin/cfpref
root               301   0.0  0.0  2491652    136   ??  Ss    5Jun18   0:00.09 /usr/libexec/sec
root               287   0.0  0.0  2515040    716   ??  S     5Jun18   0:02.39 /usr/sbin/distno
_spotlight         285   0.0  0.0  2542108   1556   ??  S     5Jun18   0:12.73 /System/Library/
root               277   0.0  0.7  3868680  55436   ??  Ss    5Jun18  14:34.84 /System/Library/
root               276   0.0  0.0  2515508    108   ??  Ss    5Jun18   0:00.09 /System/Library/
root               275   0.0  0.0  2549024   2488   ??  Ss    5Jun18   0:01.95 /System/Library/
_softwareupdate    274   0.0  0.1  4979468   4740   ??  Ss    5Jun18  95:28.52 /System/Library/
root               252   0.0  0.0  2558200    480   ??  Ss    5Jun18   0:01.14 /System/Library/
root               251   0.0  0.1  2515820   4240   ??  Ss    5Jun18  65:59.88 sysmond
root               244   0.0  0.0  2541128   1488   ??  Ss    5Jun18   0:06.39 /System/Library/
_captiveagent      241   0.0  0.0  2542100   1060   ??  Ss    5Jun18   0:05.69 /usr/libexec/cap
_networkd          236   0.0  0.1  2549100   5764   ??  Ss    5Jun18   4:21.34 /usr/libexec/sym
root               234   0.0  0.0  2456372    144   ??  Ss    5Jun18   0:00.84 /usr/sbin/cron
root               232   0.0  0.0  2516468    432   ??  Ss    5Jun18   0:05.08 /usr/sbin/cupsd
root               231   0.0  0.0  2518096    728   ??  Ss    5Jun18   0:28.06 /usr/sbin/ntpd -
root               230   0.0  0.0  2544580   1172   ??  Ss    5Jun18   0:09.23 /System/Library/
root               226   0.0  0.0  2541344   1052   ??  Ss    5Jun18   0:15.01 /usr/libexec/usb
root               225   0.0  0.0  2514532    504   ??  Ss    5Jun18   0:00.36 /usr/libexec/cor
_nsurlsessiond     223   0.0  0.1  2548980   4856   ??  Ss    5Jun18   0:18.41 /usr/libexec/nsu
root               219   0.0  0.0  2514496   1016   ??  Ss    5Jun18   0:00.64 /System/Library/
root               210   0.0  0.0  2466376    288   ??  Ss    5Jun18   0:19.38 /usr/libexec/wat
root               206   0.0  0.0  2548892   3692   ??  Ss    5Jun18   0:19.19 /usr/libexec/lsd
root               189   0.0  0.0  2515236    132   ??  Ss    5Jun18   0:00.10 /System/Library/
root               188   0.0  0.0  2544960   3324   ??  Ss    5Jun18   0:29.15 /usr/libexec/tru
root               184   0.0  0.0  2540916    276   ??  Ss    5Jun18   0:27.89 /usr/sbin/mDNSRe
_mdnsresponder     175   0.0  0.1  2543748   4680   ??  Ss    5Jun18   1:48.90 /usr/sbin/mDNSRe
root               131   0.0  0.0  2515032   2736   ??  Ss    5Jun18   0:49.79 /usr/sbin/cfpref
root               130   0.0  0.0  2543676   2300   ??  Ss    5Jun18   0:11.44 /System/Library/
root               126   0.0  0.0  2566804   3080   ??  Ss    5Jun18   0:17.50 /System/Library/
_distnote          125   0.0  0.0  2518184   1448   ??  Ss    5Jun18   0:19.68 /usr/sbin/distno
root               124   0.0  0.0  2515332   1776   ??  Ss    5Jun18   1:24.26 /usr/sbin/notify
root               123   0.0  0.0  2541824   2432   ??  Ss    5Jun18   0:07.55 /usr/libexec/Air
root               122   0.0  0.0  2516388    240   ??  Ss    5Jun18   0:00.49 /usr/libexec/cor
root               119   0.0  0.0  2473804     60   ??  Ss    5Jun18   0:00.02 /usr/sbin/Kernel
DEREK              118   0.0  0.2  2687176  20480   ??  Ss    5Jun18   1:57.26 /System/Library/
root               117   0.0  0.0  2514544    452   ??  Ss    5Jun18   0:00.38 /System/Library/
root               116   0.0  0.0  2547500   2916   ??  Ss    5Jun18   0:01.71 /System/Library/
root               111   0.0  0.0  2506800    108   ??  Ss    5Jun18   0:00.07 autofsd
root               110   0.0  0.0  2541648   2708   ??  Ss    5Jun18   0:10.52 /usr/sbin/blued
root               109   0.0  0.1  2544884   4980   ??  Ss    5Jun18   0:34.26 /usr/libexec/Due
_locationd         106   0.0  0.1  2552020   7380   ??  Ss    5Jun18   1:05.28 /usr/libexec/loc
root               104   0.0  0.0  2542292   3904   ??  Ss    5Jun18   1:42.99 /usr/sbin/securi
_usbmuxd           103   0.0  0.0  2540556   2948   ??  Ss    5Jun18   2:22.80 /System/Library/
root               102   0.0  0.1  2546184   5468   ??  Ss    5Jun18   0:59.64 /System/Library/
root               101   0.0  0.0  2541208   2364   ??  Ss    5Jun18   0:02.05 /System/Library/
root               100   0.0  0.1  2543924   6556   ??  Ss    5Jun18   1:32.61 /System/Library/
root                98   0.0  0.0  2541292   1864   ??  Ss    5Jun18   0:01.95 /usr/sbin/wirele
root                97   0.0  0.1  2565180   6604   ??  Ss    5Jun18   2:12.08 /usr/libexec/ope
root                89   0.0  0.0  2539924   2104   ??  Ss    5Jun18   0:02.97 /usr/libexec/dis
root                81   0.0  0.2  2778772  15576   ??  Ss    5Jun18   8:50.52 /System/Library/
root                79   0.0  0.0  2543860   1844   ??  SNs   5Jun18   0:02.06 /usr/libexec/war
root                78   0.0  0.1  2545548   7348   ??  Ss    5Jun18   2:54.00 /usr/libexec/air
root                74   0.0  0.1  2615032   7292   ??  Ss    5Jun18   1:54.90 /usr/libexec/log
root                68   0.0  0.0  2540652   3032   ??  Ss    5Jun18   2:18.17 /System/Library/
_appleevents        67   0.0  0.0  2542184   2312   ??  Ss    5Jun18   0:07.98 /System/Library/
root                66   0.0  0.0  2546064   4048   ??  Ss    5Jun18   2:54.34 /usr/libexec/con
root                61   0.0  0.0  2627912   2864   ??  Ss    5Jun18   3:14.50 /System/Library/
root                60   0.0  0.0  2543596   2168   ??  Ss    5Jun18   0:16.74 /usr/libexec/kex
root                59   0.0  0.0  2498588    516   ??  Ss    5Jun18   0:27.17 /System/Library/
root                56   0.0  0.1  2547568   9088   ??  Ss    5Jun18   2:00.23 /usr/libexec/Use
root                55   0.0  0.0  2516432    824   ??  Ss    5Jun18   0:39.03 /usr/sbin/syslog
root             23997   0.0  0.0  2433188   1016 s000  R+   12:53PM   0:00.00 ps aux
root                 1   0.0  0.1  2537080   8128   ??  Ss    5Jun18  15:16.59 /sbin/launchd
DEREK            23991   0.0  0.0  2452852   1588 s000  S    12:53PM   0:00.02 -bash
root             23990   0.0  0.0  2490996   2932 s000  Ss   12:53PM   0:00.02 login -pf DEREK
DEREK            23961   0.0  0.3  3321364  27776   ??  S    12:46PM   0:00.10 /Applications/Go
DEREK            23938   0.0  0.1  2505792   4292   ??  S    12:38PM   0:00.07 /System/Library/
DEREK            23857   0.0  0.0  2488328   2296   ??  Ss   12:12PM   0:00.03 /System/Library/
DEREK            23856   0.0  0.1  2520844   4972   ??  Ss   12:12PM   0:00.11 /System/Library/
DEREK            23855   0.0  1.0  1141080  86464   ??  S    12:11PM   0:25.67 /Applications/Mi
DEREK            23852   0.0  1.3  3498876 105696   ??  S    12:11PM   0:15.42 /Applications/Go
DEREK            23821   0.0  0.4  2547356  36684   ??  S    12:05PM   0:01.22 /System/Library/
DEREK            23800   0.0  0.4  2551448  30540   ??  S    12:02PM   0:01.89 /System/Library/
DEREK            23795   0.0  0.1  3059400   6784   ??  S    12:01PM   0:00.20 /System/Library/
DEREK            23793   0.0  0.0  2522820   2592   ??  S<   12:01PM   0:00.04 /Applications/At
DEREK            23782   0.0  1.0  3463144  83192   ??  S    12:01PM   0:00.93 /Applications/At
DEREK            23744   0.0  0.7  2588376  60844   ??  S    12:01PM   0:02.54 /System/Library/
DEREK            23738   0.0  2.8  3959552 231356   ??  S    12:01PM   1:46.62 /Applications/At
DEREK            23737   0.0  0.0  2481452   2368   ??  S    12:01PM   0:00.02 /Applications/At
DEREK            23733   0.0  0.6  2552612  53852   ??  S    12:01PM   0:01.71 /System/Library/
DEREK            23519   0.0  0.4  3383144  33972   ??  S    11:39AM   0:01.07 /Applications/Go
DEREK            23436   0.0  0.6  3559692  46680   ??  S    11:30AM   0:01.64 /Applications/Go
DEREK            23375   0.0  0.4  3378160  35300   ??  S    11:24AM   0:00.88 /Applications/Go
DEREK            23366   0.0  1.1  3556416  90660   ??  S    11:23AM   0:13.86 /Applications/Go
```

* Run `top` and review the results. (Hint: You may need to use `ctrl-c` to get out of this app.) *How do you interpret what you see here?* I see that the numbers are continually updating in my terminal so I believe this is a live representation of all the processes running on my laptop.

```
Processes: 328 total, 2 running, 326 sleeping, 2077 threads                                                                     12:57:07
Load Avg: 1.53, 1.76, 1.85  CPU usage: 5.5% user, 3.82% sys, 91.12% idle   SharedLibs: 160M resident, 40M data, 43M linkedit.
MemRegions: 103253 total, 2226M resident, 53M private, 781M shared. PhysMem: 8039M used (1710M wired), 145M unused.
VM: 946G vsize, 633M framework vsize, 326000(0) swapins, 410283(0) swapouts. Networks: packets: 27004633/26G in, 15490252/3712M out.
Disks: 4393228/124G read, 3008453/145G written.

PID    COMMAND      %CPU TIME     #TH   #WQ  #PORT MEM    PURG   CMPRS  PGRP  PPID  STATE    BOOSTS          %CPU_ME %CPU_OTHRS UID
24004  top          10.0 00:01.00 1/1   0    20    3244K  0B     0B     24004 23991 running  *0[1]           0.00000 0.00000    0
24001  mdworker     0.0  00:00.10 4     1    48    13M    0B     0B     24001 1     sleeping *0[1]           0.00000 0.00000    501
24000  mdworker     0.0  00:00.08 4     1    48    12M    0B     0B     24000 1     sleeping *0[1]           0.00000 0.00000    501
23999  mdworker     0.0  00:00.05 3     1    46    2976K  0B     0B     23999 1     sleeping *0[1]           0.00000 0.00000    501
23998  mdworker     0.0  00:00.18 4     1    48    21M    0B     0B     23998 1     sleeping *0[1]           0.00000 0.00000    501
23991  bash         0.0  00:00.02 1     0    16    824K   0B     0B     23991 23990 sleeping *0[1]           0.00000 0.00000    501
23990  login        0.0  00:00.02 2     1    28    1136K  0B     0B     23990 21959 sleeping *0[9]           0.00000 0.00000    0
23961  Google Chrom 0.0  00:00.10 15    1    112   13M    0B     0B     15377 15377 sleeping *0[1]           0.00000 0.00000    501
23938  mdworker     0.0  00:00.07 3     1    49    68K    0B     2980K  23938 1     sleeping *0[1]           0.00000 0.00000    501
23862  Google Chrom 0.3  00:19.46 18    2    134   94M    0B     22M    15377 15377 sleeping *0[1]           0.00000 0.00000    501
23857  com.apple.au 0.0  00:00.02 2     2    21    12K    0B     984K   23857 1     sleeping  0[0]           0.00000 0.00000    501
23856  QuickLookSat 0.0  00:00.11 2     1    45    56K    0B     3312K  23856 1     sleeping  0[2]           0.00000 0.00000    501
23855- Microsoft Wo 0.0  00:25.77 4     2    308+  47M+   12K    31M    23855 1     sleeping *0[121]         0.00000 0.00000    501
23852  Google Chrom 0.0  00:15.72 18    2    145   59M    0B     20M    15377 15377 sleeping *0[1]           0.00000 0.00000    501
23795  quicklookd   0.0  00:00.19 4     1    87    1100K  8192B  2824K  23795 1     sleeping  0[4]           0.00000 0.00000    501
23793  ShipIt       0.0  00:00.03 2     2    43    40K    0B     1384K  23793 1     sleeping *0[1]           0.00000 0.00000    501
23782  Atom Helper  0.0  00:00.93 13    1    107   1636K  0B     98M    23734 23734 sleeping *0[1]           0.00000 0.00000    501
23738  Atom Helper  0.0  02:08.53 24    1    185   130M   0B     68M    23734 23734 sleeping *0[1]           0.00000 0.00000    501
23737  crashpad_han 0.0  00:00.01 4     1    27    304K   0B     668K   23736 1     sleeping *0[1]           0.00000 0.00000    501
23734  Atom         1.1  01:59.65 38    1    407   80M+   12K    92M    23734 1     sleeping *0[430]         0.00000 0.00000    501
23647  Google Chrom 0.5  00:27.31 17    2    128   41M    0B     18M    15377 15377 sleeping *0[1]           0.00000 0.00000    501
23519  Google Chrom 0.0  00:01.08 16    2    122   2080K  0B     17M    15377 15377 sleeping *0[1]           0.00000 0.00000    501
23436  Google Chrom 0.0  00:01.65 16    1    129   5528K  0B     58M    15377 15377 sleeping *0[1]           0.00000 0.00000    501
23375  Google Chrom 0.0  00:00.89 16    2    120   2744K  0B     17M    15377 15377 sleeping *0[1]           0.00000 0.00000    501
23366  Google Chrom 0.2  00:14.29 18    2    137   45M    0B     25M    15377 15377 sleeping *0[1]           0.00000 0.00000    501
23124  periodic-wra 0.0  00:00.01 2     2    26    12K    0B     392K   23124 1     sleeping *0[1]           0.00000 0.00000    0
22996  Spotify Help 0.4  01:33.30 17    2    139   86M    0B     82M    22987 22987 sleeping *0[1]           0.00000 0.00000    501_
```

### Finding and Viewing Files

* Make sure you are in the `challenge_files` directory. Use the `*` wildcard to find all the files that have the word "credit" in the filename. *How many files did you find?*

```
2 files with credit in the filename.
credit_cards.txt:          ASCII text
credit_cards2.txt:         ASCII text
```

* Use the `more` command to view one of the `credit_cards` files you just discovered. (Hint: Type `q` to quit viewing the file. Press the `spacebar` to page down. Use your keyboard arrows to move up/down.) *What is the date in the file you have viewed?*

```
Dereks-MacBook-Pro:challenge_files DEREK$ more credit_cards.txt
Last updated: 01-15-2015
38419076308558
5196941482180427
6011648902145507
6011541522810495
2100438118121208
340330340261288
201489234446831
4486721091429528
214921348106690
2100590354720042
4539858868193585
2100183923553803
4532777298371
346539747941995
2100687370647553
869913584571073
347621194459918
4532736972558173
1800681788742606
4024007195437
374000604532174
```

* Use the `find` command to search for files more effectively. Search the sub-directories under `challenge_files` to find the location of the file named `modi_laboriosam.txt`. *Where is that file located?*

```
Dereks-MacBook-Pro:challenge_files DEREK$ find . -name modi_laboriosam.txt
./tmp/modi_laboriosam.txt
```

* Use the `grep` command to search for text within a file. Use `grep` on all the `.user` files in `challenge_files` to find which files contain "WA" (the abbreviation for Washington state). *How many files did you find?*

```
There were 2 files that were returned in my search results.

Dereks-MacBook-Pro:challenge_files DEREK$ grep "WA" *.user
Britt-Erdman.user:O'Harachester, WA 37261
Lissie-Strosin.user:Jewessfurt, WA 00816-7241
```

* Use the `-r` option of `grep` to *recursively* find the text "Waldo" hidden in a file somewhere under the `challenge_files` directory. *Paste the result showing the file and line where the word "Waldo" shows up.*

```
Dereks-MacBook-Pro:challenge_files DEREK$ grep -r "Waldo" *
serial-numbers/eaque_molestiae.txt:Ut est maiores quia autem. Nisi modi Waldo sed corporis sit explicabo ut est. Et est placeat ea sunt sunt consectetur sunt incidunt. Explicabo vel esse blanditiis dolorem culpa non quia.
```

### Pipes and Connecting Commands

* Sometimes it's useful to output the results of a command to a text file for further analysis, reference, or processing. Try running `ls > files.txt`. Notice that the file `files.txt` was created. View that file using `more`. *What do you see in the `files.txt` file?*

```
I see the names of all the files in the challenge_files directory.

Dereks-MacBook-Pro:challenge_files DEREK$ more files.txt
01
2015_special_stuff.demo
Afton-Jast.user
Aimee-Maggio.user
Alfonso-Gottlieb.user
Allen-Kemmer.user
Almina-Cormier.user
Alta-Lemke.user
Amina-McGlynn.user
Anabel-Hammes.user
Ancel-Conn.user
Anjali-Halvorson.user
Ardath-Kuvalis.user
Avah-Dickinson.user
Ayaan-Stiedemann.user
Aylin-Grant.user
Bedford-Sipes.user
Benita-King.user
Benito-Stoltenberg.user
Beverlee-Moen.user
Brad-Thiel.user
Brayan-Douglas.user
Bria-Satterfield.user
files.txt
```

* Notice that if you run `ls -alh` in the `challenge_files` directory, the files scroll by very quickly. Sometimes it would be better to get the results in a paginated format. Try running `ls -alh | more`. *Describe what you see when you run `ls -alh | more`.*

```
Dereks-MacBook-Pro:challenge_files DEREK$ ls -alh | more
total 880
drwxr-xr-x  113 DEREK  staff   3.8K Jul  4 13:31 .
drwxr-xr-x   10 DEREK  staff   340B Jul  4 11:57 ..
-rw-r--r--@   1 DEREK  staff   6.0K Jul  4 13:35 .DS_Store
drwxr-xr-x   27 DEREK  staff   918B Jul  4 10:33 01
-rw-r--r--    1 DEREK  staff     0B Jul  4 10:33 2015_special_stuff.demo
-rw-r--r--    1 DEREK  staff    93B Jul  4 10:33 Afton-Jast.user
-rw-r--r--    1 DEREK  staff    85B Jul  4 10:33 Aimee-Maggio.user
-rw-r--r--    1 DEREK  staff    79B Jul  4 10:33 Alfonso-Gottlieb.user
-rw-r--r--    1 DEREK  staff   100B Jul  4 10:33 Allen-Kemmer.user
-rw-r--r--    1 DEREK  staff    86B Jul  4 10:33 Almina-Cormier.user
-rw-r--r--    1 DEREK  staff    87B Jul  4 10:33 Alta-Lemke.user
-rw-r--r--    1 DEREK  staff    79B Jul  4 10:33 Amina-McGlynn.user
-rw-r--r--    1 DEREK  staff    78B Jul  4 10:33 Anabel-Hammes.user
-rw-r--r--    1 DEREK  staff    61B Jul  4 10:33 Ancel-Conn.user
-rw-r--r--    1 DEREK  staff    87B Jul  4 10:33 Anjali-Halvorson.user
-rw-r--r--    1 DEREK  staff    64B Jul  4 10:33 Ardath-Kuvalis.user
-rw-r--r--    1 DEREK  staff    90B Jul  4 10:33 Avah-Dickinson.user
-rw-r--r--    1 DEREK  staff    79B Jul  4 10:33 Ayaan-Stiedemann.user
-rw-r--r--    1 DEREK  staff    79B Jul  4 10:33 Aylin-Grant.user
-rw-r--r--    1 DEREK  staff    70B Jul  4 10:33 Bedford-Sipes.user
-rw-r--r--    1 DEREK  staff    82B Jul  4 10:33 Benita-King.user
-rw-r--r--    1 DEREK  staff    92B Jul  4 10:33 Benito-Stoltenberg.user
```

* Earlier, when you viewed the list of active processes on your devbox using `ps aux`, the list was probably really long. You can make this list more manageable by using the pipe (`|`) to filter the results of `ps` using `grep`. Run `ps aux | grep <your_username>` to see what processes are running for your specific user. *Paste the list of processes that reference your username here:*

```
DEREK            24137   0.0  0.0  2432804    792 s000  S+    1:48PM   0:00.00 grep Derek
```
