# Instructions to Build benchmarkdb Git folder
1. Go to projects folder, download git repo: `git clone https://github.com/milescwatson/benchmarkdb`
2. Create a directory `volumes`
3. In `volumes`, create directories `postgres` and `mysql`
4. In postgres create directory `data`, in mysql create directories `mysql-data` and `data`
5. `docker build . --tag benchmark_main --no-cache`
6. `docker-compose up`, `docker-compose up -d` for detached mode.

## Open terminal in container
Go to docker 
/mnt/wsl/docker-desktop/volumes



wsl -d docker-desktop

Potential /etc/wsl.conf fix:
```
[automount]
enabled = true
options = "metadata,umask=22,fmask=11"
```

# Github Instructions

Pull: `git pull`

Comit instructions:

add: `git add *`

commit: `git commit -a -m 'message'`

push: `git push origin development`
