## Bandit

I'm practicing Capturing the flag in OverTheWire - Bandit, Here, they hide the password in somewhere,
and we need to find it with our technical skills. I'm uploading my level completion here

  `Host : bandit.labs.overthewire.org`
  
  `Port : 2220`

  `ssh -p 2220 bandit0@bandit.labs.overthewire.org`

 - level 0 : `bandit0`  
 - level 1 : `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL` 
 - level 2 : `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`
 - level 3 : `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG`
 - level 4 : `2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe`
 - level 5 : `lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR` - find ./ -type f -size 1033c ! -executable
 - level 6 : `P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU` - find / -user username -group groupname
 - level 7 : `z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S` - cat filename.txt | grep "keyword" 
 - level 8 : `TESKZC0XvTetK0S9xNwm25STk5iWrBvP` - sort filename.txt | uniq -u  
 - level 9 : `EN632PlfYiZbn3PhVK3XOGSlNInNE00t` - strings filename.txt
 - level 10 : `G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s` - base64 -d filename.txt
 - level 11 : `6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM` - (used rot13.com to rotate the character)
 - level 12 : `JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv` - xxd(hexdump file) - file(get compressed type)
 - level 13 : `wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw` - ssh -i sshkey.private bandit14@localhost -p 2220
 - level 14 : `fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq`  - nc localhost 30000
 - level 15 : `jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt` - echo "BfMYroe26WYalil77FoDi9qh59eK5xNr" | openssl s_client -connect localhost:30001 -ign_eof
 - level 16 : `JQttfApK4SeyHwDlI9SXGR50qclOAil1` - nc localhost 3001 - 3500
 - level 17 : `VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e` - diff passwords.new passwords.old
 - level 18 : `hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg` -  ssh -p 2220 bandit18@bandit.labs.overthewire.org cat "readme"
 - level 19 : `awhqfNnAbc1naukrpqDYcF95h7HoMTrC` -  ./bandit20-do cat /etc/bandit_pass/bandit20
 - level 20 : `NvEJF7oVjkddltPSrdKEFOllh9V1IBcq` -  echo -n "VxCazJaVykI6W36BkBU0mJTCM8rR95XT" | nc -l -p 1234  &
 - level 21 : `WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff` - cat /usr/bin/cronjob_bandit22.sh
 - level 22 : `QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G` - echo I am user bandit23 | md5sum | cut -d ' ' -f 1
 - level 23 : `VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar` - echo "cat /etc/bandit_pass/bandit24 > /tmp/rand/password" > shellfile.sh 
 - level 24 : `p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d` - for i in {0000..9999}; do echo VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar $i; done | nc localhost 30002
 - level 25 : `c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1` - :set shell =/bin/bash, :shell
 - level 26 : `YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS` - ./bandit27-do cat /etc/bandit_pass/bandit27
 - level 27 : `AVanL161y9rsbcJIsFHuw35rjaOM19nR` - git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo
 - level 28 : `tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S` - git log , git show
 - level 29 : `xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS` - git branch , git checkout , git log -p - l 
 - level 30 : `OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt` - git tag
 - level 31 : `rmCBvG56y58BXzv98yZGdO7ATVL5dW8y` - git push origin master
 - level 32 : `odHo63fHiFqcWWJG9rLiLDtPm45KzUKy` - git tag, git show secret
 - level 33 : `completed` 
