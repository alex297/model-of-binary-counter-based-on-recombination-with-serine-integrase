# model-of-binary-counter-based-on-recombination-with-serine-integrase
Matlab files of a model described in a paper "A single-input binary counting module based on serine integrase  site-specific recombination" NAR, 2019, by Jia Zhao, Alexandra Pokhilko, Oliver Ebenhöh, Susan J. Rosser, and Sean D. Colloms.
Institute of Molecular, Cell and Systems Biology, University of Glasgow, Bower Building, Glasgow G12 8QQ

To simulate latch kinetics - run tetR_110219.m; figure(1) draws kinetics, figure(2) draws phase diagram; requires ODE file Model_tetR_110219.m

Fig. 5: run tetR_110219.m with t=[0 2], kt=0.03 (default kt=0.3), araon=0.5, araoff=0.7. For Fig. S5B,C: Ktet=10, for Fig. 5E,F: Ktet=0.01. Initial conditions: Fig. 5B - y0=[0*Dtot 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1*Dtot 0 0 0 0 0 0 0 0 0 0 0 0 0 0], Fig. 5E - y0=[0*Dtot 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1*Dtot 0 0 0 0 0 0 0 0 0 0 0 0 0.4 0.06], Fig. 5C,F - y0=[Dtot 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 0*Dtot 0 0 0 0 0 0 0 0 0.5 0 0 0 0 0].

Fig. S10: run tetR_3D_110219.m for Fig. S10A-C; run tetR_3D_110219_int.m for Fig. S10D. Requires many hours of run, for faster runs reduce t.

Fig. S11: run tetR_110219.m with t=[0 24*5], araon=2.5, araoff=2.7. Initial conditions: Fig. S11A - y0=[0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0.01,Dtot,0,0,0,0,0,0,0,0,0.005,0,0,0,0.4,0.05], Fig. S11B - y0=[1*Dtot,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0.5,0*Dtot,0,0,0,0,0,0,0,0,0.25,0,0,0,0.06,0.01], Fig. S11C - y0=[0.6*Dtot,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0.5,0.4*Dtot,0,0,0,0,0,0,0,0,0.25,0,0,0,0.06,0.01], Fig. S11D - figure(2) under initial conditions of Fig. S11A,B,C.

For simulations of plasmid segregation:

Fig. 6B: run pl_segr_110219.m

Fig. S13: run pl_segr_110219_hist.m with LR=3/20 (Fig. S14A,B); LR=10/20 (Fig. S14C,D); LR=17/20 (Fig. S14C,D).
Fig. S14: run tetR_110219.m with araon=0.5, araoff=0.7. Initial run - t=[0 24*6] to reach steady state; final run t=[0 24*4]; parameter period equal to 18, 14, 10, 6, 2 for panels A-E.

