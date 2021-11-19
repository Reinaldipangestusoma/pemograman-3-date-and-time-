# pemograman-3-date-and-time-
reinaldi pangestu soma

#eskplor Mendapatkan tanggal saat ini
import datetime
tanggal_saat_ini = datetime.date.today() 
print(tanggal_saat_ini) # tanggal pada hari ini akan ditampilkan di layar


#eskplor Mendapatkan tanggal dan waktu saat ini
import datetime
saat_ini = datetime.datetime.now() 
print(saat_ini) # waktu saat ini akan ditampilkan di layar


#eskplor Mengisi variabel dengan tanggal tertentu
from datetime import date
tgl = date(2019, 7, 31) # tahun, bulan, tanggal
print(tgl)


#eksplor Mengakses tahun, bulan, tanggal dari sebuah date object
from datetime import date
hari_ini = date.today() 
print("Tahun ini:", hari_ini.year)
print("Bulan ini:", hari_ini.month)
print("Tanggal hari ini:", hari_ini.day)


#eksplor Mengisi variabel dengan waktu tertentu
from datetime import time
cth_waktu = time(20, 31, 7) # parameter: jam, menit,detik
print(cth_waktu)
cth_waktu = time(hour = 8, second = 56) # 
print(cth_waktu)
cth_waktu = time(1, 11, 27, 991727) # parameter: jam, menit,detik, microsecond
print(cth_waktu)


#eksplor Mengakses jam, menit, detik, dan microsecond dari sebuah time object

from datetime import time
a = time(5, 15, 5, 728172)
print("jam =", a.hour)
print("menit =", a.minute)
print("detik =", a.second)
print("microsecond =", a.microsecond)


#eksplor Menghitung selisih antara dua tanggal

from datetime import date
tgl1 = date(year = 1945, month = 8, day = 17)
tgl2 = date.today()
selisih = tgl2 - tgl1
print('Indonesia sudah merdeka selama =', selisih.days, ' hari')
catatan: selisih pada contoh di atas bertipe timedelta

#eksplor Format tanggal dan waktu dengan strftime

from datetime import datetime
saat_ini = datetime.now()
jam = saat_ini.strftime('%H:%M:%S')
print('Jam:', jam)
tgl = saat_ini.strftime('%d/%m/%Y') # format dd/mm/YY
print('Tanggal:', tgl)
tgl_jam = saat_ini.strftime("%d/%m/%Y, %H:%M:%S") # format dd/mm/YY H:M:S 
print('tanggal dan jam: ', tgl_jam)
