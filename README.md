


For each of the 32 states, execute the R script files in the following order:

1. **state_precint_manipulation.R**
   > Takes elections from 2004 up until 2019 and manipulates and generates vote data in absolute terms.
   >
   > It identifies with a unique id each municipality from the state, aggregating and appending all elections.

2. **vote_manipulation.R**
   > From the previously created vote database, this script organizes and selects the desired variables for further cleaning.

3. **incumbent_manipulation.R**
   > This file then manipulates and runs the incumbent candidate information merging the incumbent party and candidate data into the vote data.

4. **incumbent_vote_calculator.R**
   > Given the final values of incumbent parties and the corresponding vote values, the script proceeds to calculate incumbent and runner-up votes in absolute terms.

5. **final.R**
   > This script generates the final version of the incumbent vote data for each state.
   >
   > It calculates the state incumbent vote values, as well as the values for votes for MORENA, PAN, PRI, PRD.
   >
   > **Important**: Run the corresponding `state_collapsed_edited` file to correctly execute the tasks in the script.
   >
   > The above-described files can be found in: **`Data -> collapsed database manual cases`**
   > 
**                                                                                                                       **
   **Only after executing the files from steps 1 through 5 for each of the 32 states, then execute the R script in step 6 below:**
**                                                                                                                       **
     
6. **FINAL_db_formation.R**
    > This is the final step, as it consolidates the final version of each of the 32 states into a single file, and then proceeds to clean it and calculate the vote shares based on: "lista nominal" which is the vote registry, and "valid" which are valid votes. 
