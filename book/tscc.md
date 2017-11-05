# TSCC Tips 
* `qsub -t` to submit multiple jobs to queue 
* Use `qalter -W queue=[] -l walltime=xx` to change queue and walltime 
* `qsub -W depend=afterany:jobid` to submit job after any old job terminated. `jobid` can be a whole job array `xx[]` or member of a job array `xx[1]`


