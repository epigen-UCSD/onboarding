# TSCC Sever guide 

## infrastructure 

1. tscc-server: major computing horsepowers. 
2. vm-server: webserver soly used for develop web applications and data sharing purpose.
3. data storage (`/project/ps-epigen'): permanent data storage location.




## Submitting jobs 

## Software

## Tips

* `qsub -t` to submit multiple jobs to queue 
* Use `qalter -W queue=[] -l walltime=xx` to change queue and walltime 
* `qsub -W depend=afterany:jobid` to submit job after any old job terminated. `jobid` can be a whole job array `xx[]` or member of a job array `xx[1]`


