## Title: Emergency Room Waiting Simulation
### Team Member(s): Nanzhu Liu & Qiuyan Guo

## Monte Carlo Simulation Scenario & Purpose:
- This project is to make simulations for the nurse & doctor v.s. patients situation in an emergency room of a hospital, to see the utilization of nurses and doctors, and the waiting time of patients.
  ### Assumptions:
  - The numbers of nurses and doctors are assigned at any given time, no breaks or shift time waste for these nurses and doctors
  - The approximate patient number per hour is assigned, the exact patient number will be within 2 people of the given number
  - All of the patients will see a nurse first, 20% of them will leave after seeing the nurse, the rest of them will also see a doctor after the nurse
  - Time spending with a nurse and a doctor both follow the same normal distribution, with the assigned mean time value, sd = 1, min/max = mean -/+ 10
  - All time-related values are in minute(s)

## Simulation's variables of uncertainty:
  ### Random variables:
  - Exact patient numbers in an hour
  - The arrival time of each patient in the hour
  - Either a patient comes only to see a nurse or to see both a nurse and a doctor
  - The time(minutes) a nurse / doctor spent with a patient

## Hypothesis or hypotheses before running the simulation:
- When utilization results > 1, patients must need to wait for nurse or doctor, vice versa

## Analytical Summary of findings: 
- We indeed needed to change the assumptions several times based on the simulation outcomes during the process
- With each set of numbers, the results remain stable after 20000 times of simulations
- When utilization results > 1, it's highly possible that patients need to wait nurse and doctor, but not necessarily
- The higher the utilization rates go, the longer patients tend to wait

## Instructions on how to use the program:
- Run the main.py file, which contains the complete program with utilization and waiting time calculations
- When calling the simulation function in the main function, change the values of the parameters refering to numbers of nurses, doctors, patients, time a nurse/doctor spent with a patient, and running times, to get different results
- Example_plots.ipynb contains same algorithm, only to show an example of the plots based on one set of people numbers
- Output.txt contains printed results of the similuations of several sets of people numbers currently in the main.py file as examples

### Tasks:
- Time distribution, Utilization calculation - Nanzhu Liu
- Waiting time calculation - Qiuyan Guo
