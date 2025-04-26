# Scheduling problem description
This is my python of scheduling problem in flexible flowshop (many stages, many machines each stage)
The system has four stage, with many parallel machine each stage. All of jobs will be assigned simultaneously in machines and go through all the stages. In this problem, we need to consider 2 fields: job perspective and machine perspective.
The work will be divided into equal parts on parallel machines, all of sub-job start and finish at the same time. 
Unlike other problems, the next stage does not start from the completing time of the previous stage but from the time the previous stage produces enough WIP for the this stage. At machines of the first stage, the job is started after job's release time and the completing time of previous job. At each machine of other stages, starting time of job is after the the completing time of previous job and the minimum time of the job at previous stage to produce enough WIP.
Objective is minimun Laterness.
