# Arquivo PY

import re

with open('logs.txt', 'r', encoding='utf-8') as file:
    arq = file.readlines()

for line in arq:
    print(line[:-1])
    x = re.findall(r'\. [a-zA-Zã\. ]+ -', line)
    result = x[0]
    print(result[ 2:-2 ])
    print('--')

