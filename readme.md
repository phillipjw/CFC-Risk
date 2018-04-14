# CFC Compliance Detector
Checks whether or not a given subsidiary complies with the new CFC regulations beginning Jan 1, 2019
Generates simulated subsidiaries and checks their compliance. If CFC violation detected returns the home country tax that would be paid.

### Requirements

run the following in the cloned folder
```
pip install -r requirements.txt
```

### Running

To generate a simulated corporation and check its CFC compliance run the block
```
import os

size = corporation_size
output = np.zeros(shape = (size, 4))

for i in range(size):
    output[i,:] = decision_procedure(gen_subsidiary())

np.savetxt(os.getcwd()+'/output.csv', output, delimiter=',')
```
### Authors
Phillip Wozny
Sam Jing
Rashimil



