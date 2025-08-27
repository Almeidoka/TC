# Arquivo PY

import re

with open('logs.txt','r', encoding='utf-8') as file:
  arq = file.readlines ()

for line in arq:
  print(line[:-1])
  x = re.findall(r'[0-9][0-9][0-9]\.?\d\d\d\.?\d\d\d-?\d\d', line)
  print('--')
