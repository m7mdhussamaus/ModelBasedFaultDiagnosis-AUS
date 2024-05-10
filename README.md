Model Based Fault Diagnosis

This repository contains Python scripts for model-based fault diagnosis using Finite State Machines (FSMs). The scripts generate mutants of an FSM, simulate these mutants against a suite of tests, and filter out non-unique mutants based on their behavior.

Project Structure



To run the scripts, you will need Python 3.6 or higher. Clone this repository to your local machine:

bash
Copy code
git clone https://github.com/yourusername/model-based-fault-diagnosis.git
cd model-based-fault-diagnosis
Usage

To execute the main script, you need to specify the paths to your FSM configurations and the test suite directory. Ensure you update these paths in the main.py script according to your directory structure:

Edit File Paths:
Open main.py and modify the fsm_filepath and test_suite_directory variables to point to your specific files and directories.
python
Copy code
# Example file paths setup in main.py
fsm_filepath = '/path/to/your/mutants.txt'
test_suite_directory = '/path/to/your/test/suite/directory'
Run the Script:
Execute the script from the command line.
bash
Copy code
python src/main.py
This command will run the simulations and generate a file mutants.txt in the root directory, containing all unique FSM mutants.

Modifying the Code

If you need to adjust the simulation or mutation logic:

Navigate to src/ and modify main.py as per your requirements.
You can increase or decrease the number of mutants generated or change the mutation logic within the generate_mutants function.
Contributing

Feel free to fork this repository and submit pull requests. You can also open an issue if you find any bugs or have suggestions for further enhancements.
