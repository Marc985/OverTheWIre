## level 0
    ->ssh bandit0@bandit.labs.overthewire.org -p 2220
    ->cat readme.txt 
   
Password:bandit0

---

## level 0->1
    ->ls
    ->cat readme.txt

Passeword:NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

---

## level 1->2

   ->ssh bandit1@bandit.labs.overthewire.org -p 2220
   -> cat ./-

Passeword:rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

---


## level 2->3
   
   ->ls
   ->cat 'spaces in this filename'

Passeword:aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

---


## level 3->4
   
    ->cd inhere
    ->ls -a 
    ->cat .hidden
 
 Passeword:2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

---


 ## level 4->5
   
   ->file ./*
   ->cat ./-file07

Passeword:lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

---

## level 5->6
   
   ->find . -size 1033c
   ->cat ./maybehere07/.file2

Passeword:P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

---

## level 6->7
  
  ->find / -user bandit7 -group bandit6 -size 33c
  ->cat /var/lib/dpkg/info/bandit7.password

Passeword:z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

---

## level 7->8
  
  ->grep millionth data.txt

Passeword:TESKZC0XvTetK0S9xNwm25STk5iWrBvP

---

## level 8->9
  
  ->cat data.txt | sort  | uniq -u

Passeword:EN632PlfYiZbn3PhVK3XOGSlNInNE00t

---

## level 9->10
  
  ->string data.txt | grep ===

Passeword:G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

---

## level 10->11
 
 ->cat data.txt | base64 -d

Passeword:6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

---

## level 11->12

   ->cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

Passeword:JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

---

## level 12->13

  ->mkdir /tmp/bandit12
  ->cd /tmp/bandit12
  ->cp data.txt /tmp/bandit12
  ->cat data.txt | xxd -r data
  ->file data
 
  ->mv data data2.gz
  ->gzip -d data2.gz 
  ->file data2
  ->mv data2 data3.bz
  ->file data3
  ->mv data3 data4.gz
  ->gzip -d data4.gz
  ->file data4
  ->mv data4 data5.tar
  ->ls
  ->file data5.bin
  ->mv data5.bin data6.tar
  ->tar -xf data6.tar
  ->ls
 
  ->file data6.bin
 data6.bin: bzip2 compressed data, block size = 900k
  ->mv data6.bin data7.bz
  ->bzip2 -d data7.bz
  ->ls
 
  ->file data7

  ->mv data7 data8.tar
  ->tar -xf data8.tar
  ->ls 

  ->file data8.bin
  
  ->mv data8.bin data9.gz
  ->gzip -d data9.gz
  ->file data9
 data9: ASCII text(The password is stored in an ASCII file)
  cat data9

Passeword:wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw

---

## level 13 ->14

  ->ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
  ->cat /etc/bandit_pass/bandit14

Passeword:fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

---

## level 14->15

  ->echo "fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq" | nc localhost 30000

Passeword:jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt

---

## level 15->16

  ->echo "jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt" | openssl s_client -connect localhost:30001 ign_eof

Passeword:JQttfApK4SeyHwDlI9SXGR50qclOAil1
 