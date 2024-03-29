Update 29 March 

The YAML file show different ways to load S (as well as many other parameters) in SeisSol

With ASAGI: 
-
  stress_field_aochi58_ASAGI.yaml
  le-teil_stress_seissol_f4.nc (netCDF file stored sig_zz and S)


With built-in FunctionMAP: 
-
  stress_field_d58_p1.yaml (fit S with polynomial degree = 1)
  stress_field_d58_p2.yaml (fit S with polynomial degree = 2)

###

Test on dc: 
-
First test: (at the center of the circular patch, dc is 0.01 cm, it linearly increases to 0.05 cm at the patch boundary, with a rate of increase of 0.00004 cm per meter)

  sphere_test_dc_S02.yaml 
  stress_field_aochi_S_0.2.yaml

Second test: (at the center of the circular patch, dc is 0.05 cm, it linearly decreases to 0.01 cm at the patch boundary, with a rate of increase of 0.00004 cm per meter)

  sphere_test_dc_S02.yaml
  stress_field_aochi_S_0.2.yaml
