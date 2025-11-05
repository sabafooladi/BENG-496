
# BENG 469 Lab session 7-2 - instructions

#### Open OOD in a browser window
https://beng469f.ycrc.yale.edu/
 
<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/ood1.png" alt="foo bar" title="train &amp; tracks" /></p>

Click **Clusters** -> **shell access**

<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/bouchet.png" alt="foo bar" title="train &amp; tracks" /></p>


Go to your results under **project** fileset to Check the log file for STPipeline

```
cd /nfs/roberts/project/beng469f/beng469f_NETID/Lab7-Spatial_transcriptomics/50t/
```

Use ls command to list files and directories.
```
ls -lrt 
```
<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/3.png" alt="foo bar" title="train &amp; tracks" /></p>

```
cat 50t_log.txt
```
<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/4.png" alt="foo bar" title="train &amp; tracks" /></p>

<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/5.png" alt="foo bar" title="train &amp; tracks" /></p>

<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/6.png" alt="foo bar" title="train &amp; tracks" /></p>


Go to **Lab7-Spatial_transcriptomics** directory
```
cd /nfs/roberts/project/beng469f/beng469f_sf882/Lab7-Spatial_transcriptomics/
```

#### Copy ipynb file to you folder
```
cp /nfs/roberts/project/beng469f/shared/Lab7/Lab7-SpatialDE.ipynb ./
```

Start an interactive job

```
salloc
```

```
module load miniconda
```

```
conda create -y -n spatialde python=3.7
```

```
conda activate spatialde
```

```
pip install numpy pandas matplotlib jupyter patsy
```

```
pip install spatialde
```


```
module purge
```

```
ycrc_conda_env.sh update
```

```
cd ~/ondemand
```

```
ls -lrt
```

```
cat conda-jupyter-env-list.txt
```

---

#### Launch a Jupyter session:

   
Go to the Jupyter initialization page, and specify the parameters/resources as follows:

| Parameters      | Values |
| ----------- | ----------- |
| version      | Conda:spatialde       |
| Number of hours   | 6        |
| Number of CPU cores per node   | 1       |
| Memory per CPU core in GiB   | 8       |
| Partitions   | education        |

<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/7.png" alt="foo bar" title="train &amp; tracks" /></p>


<p><img width="1000" src="https://github.com/sabafooladi/BENG-496/blob/main/Lab7-2/8.png" alt="foo bar" title="train &amp; tracks" /></p>


### [SpatialDE](https://www.nature.com/articles/nmeth.4636)
