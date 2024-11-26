# Diversity Optimization for Travelling Salesman Problem via Deep Reinforcement Learning
RF-MA3S is a solver capable of solving query route tasks such as Traveling Salesman Problem (TSP) and Capacitated Vehicle Routing Problem (CVRP). After processing the instances, the solution set obtained exhibits a favorable balance between diversity and optimality. This solver is based on novel designs, including:

- Relativization Filter (RF): It is designed to enhance the encoder’s robustness against affine transformations (translation, rotation, scaling, and mirroring) of the input data, ingeniously embedding explicit invariance to potentially improve the quality of the discovered solutions.<br>
- Multi-Attentive Adaptive Active Search (MA3S): It is tailored to enable the decoders to learn or mine data within different solution spaces, striking a balance between optimality and diversity.

![image](https://github.com/user-attachments/assets/ab9ba163-1fed-4c78-8142-0fe6bb0197ee)

# Dependencies
```
python = 3.8.13
pytorch = 2.0.0 
numpy
```

# Usage


# Acknowledgements

The code and the framework are based on [POMO](https://github.com/yd-kwon/POMO/tree/master):
```
@inproceedings{NEURIPS2020_f231f210,
 title = {POMO: Policy Optimization with Multiple Optima for Reinforcement Learning},
 author = {Kwon, Yeong-Dae and Choo, Jinho and Kim, Byoungjip and Yoon, Iljoo and Gwon, Youngjune and Min, Seungjai},
 booktitle = {Advances in Neural Information Processing Systems},
 volume = {33},
 pages = {21188--21198},
 year = {2020}
}
```


# Additional Notes
The **test data** folder contains:

(1) [MSTSPLIB](https://github.com/GnauhGnit/MSTSP) , <br>

![image](https://github.com/user-attachments/assets/fd2d45cd-43d2-4c08-bcb6-ba25ea454965)

(2) [TSPLIB](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp/) , <br>
(3) [CVRPLIB](http://vrp.galgos.inf.puc-rio.br/index.php/en/).

# Inspiration for Future Work
Using an improvement-method for Diversity Optimization rather than a construction-method might be a promising direction.Such as:
```
@inproceedings{NEURIPS2023_9bae70d3,
 author = {Ma, Yining and Cao, Zhiguang and Chee, Yeow Meng},
 booktitle = {Advances in Neural Information Processing Systems},
 editor = {A. Oh and T. Naumann and A. Globerson and K. Saenko and M. Hardt and S. Levine},
 pages = {49555--49578},
 publisher = {Curran Associates, Inc.},
 title = {Learning to Search Feasible and Infeasible Regions of Routing Problems with Flexible Neural k-Opt},
 url = {https://proceedings.neurips.cc/paper_files/paper/2023/file/9bae70d354793a95fa18751888cea07d-Paper-Conference.pdf},
 volume = {36},
 year = {2023}
}
```
And RCC in LEHD:
```
@inproceedings{NEURIPS2023_1c10d0c0,
 author = {Luo, Fu and Lin, Xi and Liu, Fei and Zhang, Qingfu and Wang, Zhenkun},
 booktitle = {Advances in Neural Information Processing Systems},
 editor = {A. Oh and T. Naumann and A. Globerson and K. Saenko and M. Hardt and S. Levine},
 pages = {8845--8864},
 publisher = {Curran Associates, Inc.},
 title = {Neural Combinatorial Optimization with Heavy Decoder: Toward Large Scale Generalization},
 url = {https://proceedings.neurips.cc/paper_files/paper/2023/file/1c10d0c087c14689628124bbc8fa69f6-Paper-Conference.pdf},
 volume = {36},
 year = {2023}
}
```



# License

[MIT](LICENSE) © Richard Littauer

