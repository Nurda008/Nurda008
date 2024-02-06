import psutil
for k, v in psutil.net_if_addrs().items():
for item in v:
address = item[1]
if '.' in address and len(address) <= 15:
print(k)
print(address)
