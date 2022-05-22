duration = int(input(' Введите число: '))
s = 1
m = 60
h = 3600
d = 86400

if duration < 60:
  print(duration // s, 'sec')
elif duration > 59 and duration < 3600:
  print(duration // m, ' min ', duration % m, 'sec')
elif duration > 3599 and duration < 86400:
  print(duration // h, 'hour', (duration // m) % m, 'min', duration % m, 'sec')
elif duration >= 86400:
  print(duration // d, 'day', (duration // h) % h, 'hour', (duration // m) % m, 'min', duration % m, 'sec')
  
