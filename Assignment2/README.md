
#  BENG 469 Assignemnt 2 - instructions

##  Part 1: Run stpipeline on another sample (GSM4096261_10t)
1. Access the Bouchet cluster
  <p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/bouchet.png" alt="foo bar" title="train &amp; tracks" /></p>

2. Go to the Lab7-Spatial_transcriptomics directory:
```bash
cd /nfs/roberts/project/beng469f/beng469f_NETID/Lab7-Spatial_transcriptomics/
```
3. Create a new diretory named 'Assignment2':
```bash
mkdir Assignment2
```
4. Go to the Assignment2 directory:
```bash
cd Assignment2
```
5. Copy the stpipeline-Assignment2.sh to your folder:
```bash
cp /nfs/roberts/project/beng469f/shared/Assignment2/stpipeline-assignment2.sh ./
```

6. Copy .ipynb file to you folder:
```bash
cp /nfs/roberts/project/beng469f/shared/Assignment2/Lab7-SpatialDE-Assignment2.ipynb ./
```


7. Start an interactive job:
```bash
(leave as blank on purpose)
```

8. Load Miniconda and activate the conda environment 'st-pipeline':
```bash
(leave as blank on purpose)
```

9. Submit the job to the compute node:

Replace NETID with your netid (don’t need to add beng469) and your email address.
```bash
sbatch stpipeline-Assignment2.sh NETID --mail-user=xx.xx@yale.edu
```

Pause and wait for the job to finish (approximately 3 hours). After receiving an email confirming job completion, proceed to Part 2.

11. Check the output directory:

$\color{red}{\textsf{If you successfully finish Part 1, when you run the following command}}$

```bash
ls -lrt /nfs/roberts/project/beng469f/beng469f_$NETID/Lab7-Spatial_transcriptomics/Assignment2/10t/
```

$\color{red}{\textsf{You will get 5 files:}}$

<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Assignment2/10.png" alt="foo bar" title="train &amp; tracks" /></p>


###  Part 2: Finish 5 code writing/completion tasks in the Jupyter notebook


1. Open OOD and Launch an Jupyter session with the following parameters:

| Parameters      | Values |
| ----------- | ----------- |
| Environment Setup (select the miniconda environment) | spatialde  |
| Number of hours   | 6        |
| Number of CPU cores per node   | 1        |
| Memory per CPU core in GiB   | 8       |
| Partitions   | education        |


2. Open the Jupyter notebook (Project-> Lab7-Spatial_transcriptomics -> Assignment2 -> Lab7-SpatialDE-Assignment2.ipynb)

3. complete the 5 tasks.

4. Save the .ipynb file after you finish.

5. Check the Assignment2 directory for files:

$\color{red}{\textsf{You don’t need to submit any additional file or report for this assignment.}}$ 

$\color{red}{\textsf{If you successfully finish Part 2, go back to the clusters, and run the following command:}}$
```
ls -lrt /nfs/roberts/project/beng469f/beng469f_sf882/Lab7-Spatial_transcriptomics/Assignment2
```


$\color{red}{\textsf{You will get these files:}}$

<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Assignment2/11.png" alt="foo bar" title="train &amp; tracks" /></p>

We will evaluate the results from those files.

