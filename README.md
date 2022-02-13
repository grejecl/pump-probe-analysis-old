**ppa** - (*Pump-probe analysis*) - module for analysis, visualization and fitting of ultrafast transient reflectivity time-traces, written in python.  

---

Fitting with DECP-like models [1] proceeds in two steps: 
1) [Differential Evolution algorithm](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.differential_evolution.html) is used to obtain a rought estimate of optimal parameters,
2) Data is further fit with [least-squares algorithm](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.curve_fit.html?highlight=curve_fit) (trf or lm method) using previously estimated parameters as initial guess. 

See *ppa_example.py* for a demonstration. 

---

This project is no longer maintained. Written a long time ago hence multiple issues: functional paradigm only; originally made to be run as script and doesn't work well with jupyter; generally barely sufficient at best.


[1] H.J. Zeiger et. al., Theory for displacive excitation of coherent phonons, Phys. Rev. B 45, 768.
