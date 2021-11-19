# pemograman-3-date-and-time-
reinaldi pangestu soma

from datetime import datetime
saat_ini = datetime.now()
jam = saat_ini.strftime('%H:%M:%S')
print('Jam:', jam)
tgl = saat_ini.strftime('%d/%m/%Y') # format dd/mm/YY
print('Tanggal:', tgl)
tgl_jam = saat_ini.strftime("%d/%m/%Y, %H:%M:%S") # format dd/mm/YY H:M:S 
print('tanggal dan jam: ', tgl_jam)
