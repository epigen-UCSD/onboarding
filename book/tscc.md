# TSCC Sever guide 

## infrastructure 

1. tscc-server: major computing horsepowers. 
2. vm-server: webserver soly used for develop web applications and data sharing purpose.
3. data storage (`/project/ps-epigen'): permanent data storage location.

## Conda 

### Users
Each user need to  set the personal config file `~/.condarc`:

``` shell
pkgs_dirs:
- ~/.conda/pkgs
```

Then create environment by using:
1. `env_name.txt`
2. `conda create -n xxx -c chanels ... --file env_name.txt`

User need to maitain the `env_name.txt` and can request conda admin to install the personal environment into the shared space. 


### commands 
* Update conda `conda update -n base conda`


## Submitting jobs 

## Software

## Tips

* `qsub -t` to submit multiple jobs to queue 
* Use `qalter -W queue=[] -l walltime=xx` to change queue and walltime 
* `qsub -W depend=afterany:jobid` to submit job after any old job terminated. `jobid` can be a whole job array `xx[]` or member of a job array `xx[1]`


