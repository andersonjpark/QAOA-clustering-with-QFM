# QAOA-clustering-with-QFM

Announcement: I am currently running the actual hardware backend using Qiskit so the code and result will be uploaded by end of July.

# Report

## Abstract 

Finding the global solution to combinatorial optimization problems is NP-hard and it becomes much more diﬃcult as the problem size grows. Howver, these problems have many applications in the industry and there has been attempts to ﬁnd the global solution in many areas. Quantum computing is also an area that presents possibility of solving combinatorial problems since they can easily be mapped to an Ising Hamiltonian problem.

There has been papers that shows how to transform clustering problems to a QUBO problem, and then solve with Quantum Approximate Optimization Algorithm (QAOA) [1]. The geometry of data becomes especially important for clustering since clustering algorithms operate based on the distance between data points. The distance between data points transform in to a weight of an edge that connects vertices when translated to a combinatorial optimization problem on a graph.

It has been shown in Refs. [2,3] that quantum feature maps can solve clustering problems that are hard to do with classical distances.

Project problems were 

1. Find an interesting clustering problem and solve it via QAOA while using the Euclidean distance to construct the corresponding graph.

2. Use quantum feature maps (or quantum kernels) to determine the distances between data points. Perform clustering again via QAOA and compare the results obtained under diﬀerent distances.

In this repository, we hope to present two trends.

First, we will be showing increase in accuracy and decrease in cost function proportional to the number of layers (p) when attempting K-means clustering with weighted graph using QAOA.

Second, we will present the beneﬁt of using Quantum Feature Mapping for non-clustered data points which leads to increase in versatility of various clustering algorithms.

## Results

## Discussion

Due to time and technological diﬃculties, we weren't able to present the result with bigger parameters. We couldn't run the simulation in much more complicated data points due to the limitation of qubits, performance of computer, and time limitation. In the future, we would hope to present results with deeper depth in circuits, and bigger datasets with more qubits.

References

[1] Johannes S Otterbach, Riccardo Manenti, Nasser Alidoust, A Bestwick, M Block, B Bloom, S Caldwell, N Didier, E Schuyler Fried, S Hong, et al. Unsupervised machine learning on a hybrid quantum computer. arXiv preprint arXiv:1712.05771, 2017.

[2] Yudai Suzuki, Hiroshi Yano, Qi Gao, Shumpei Uno, Tomoki Tanaka, Manato Akiyama, and Naoki Yamamoto. Analysis and synthesis of feature map for kernel-based quantum classiﬁer. Quantum Machine Intelligence, 2(1):9, July 2020.

[3] Vojtech Havl´ıcek, Antonio D. C´orcoles, Kristan Temme, Aram W. Harrow, Abhinav Kandala, Jerry M. Chow, and Jay M. Gambetta. Supervised learning with quantumenhanced feature spaces. Nature, 567(7747):209–212, 2019.

[4] MacQueen, J. B. (1967). Some Methods for classiﬁcation and Analysis of Multivariate Observations

[5] Qiskit: Aleksandrowicz, G., Alexander, T., Barkoutsos, P., Bello, L., BenHaim, Y., Bucher, D., Cabrera-Hern´andez, F.J., Carballo-Franquis, J., Chen, A., Chen, C.F., Chow, J.M., C ´orcoles-Gonzales, A.D., Cross, A.J., Cross, A., Cruz-Benito, J., Culver, C., Gonz´alez, S.D.L.P., Torre, E.D.L., Ding, D., Dumitrescu, E., Duran, I., Eendebak, P., Everitt, M., Sertage, I.F., Frisch, A., Fuhrer, A., Gambetta, J., Gago, B.G., Gomez-Mosquera, J., Greenberg, D., Hamamura, I., Havlicek, V., Hellmers, J., Herok, Ł., Horii, H., Hu, S., Imamichi, T., Itoko, T., Javadi-Abhari, A., Kanazawa, N., Karazeev, A., Krsulich, K., Liu, P., Luh, Y., Maeng, Y., Marques, M., Mart´ın-Fern´andez, F.J., McClure, D.T., McKay, D., Meesala, S., Mezzacapo, A., Moll, N., Rodr´ıguez, D.M., Nannicini, G., Nation, P., Ollitrault, P., O’Riordan, L.J., Paik, H., P´erez, J., Phan, A., Pistoia, M., Prutyanov, V., Reuter, M., Rice, J., Davila, A.R., Rudy, R.H.P., Ryu, M., Sathaye, N., Schnabel, C., Schoute, E., Setia, K., Shi, Y., Silva, A., Siraichi, Y., Sivarajah, S., Smolin, J.A., Soeken, M., Takahashi, H., Tavernelli, I., Taylor, C., Taylour, P., Trabing, K., Treinish, M., Turner, W., Vogt-Lee, D., Vuillot, C., Wildstrom, J.A., Wilson, J., Winston, E., Wood, C., Wood, S., W¨orner, S., Akhalwaya, I.Y., Zoufal, C.: Qiskit: An open-source framework for quantum computing (2019)

[6] Fowlkes-Mallows score: Fowlkes, E. B.; Mallows, C. L. (1 September 1983). "A Method for Comparing Two Hierarchical Clusterings". Journal of the American Statistical Association. 78 (383): 553. doi:10.2307/2288117

[7] PennyLane: Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, Carsten Blank, Keri McKiernan and Nathan Killoran. PennyLane. arXiv, 2018. arXiv:1811.04968

[8] Scikit-learn: Pedregosa F et al 2011 J. Mach. Learn. Res. 12 2825–30
