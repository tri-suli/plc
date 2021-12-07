# Personal Learning Score
Untuk memotivasi siswa konsisten belajar, Ruangguru membuat fitur gamification baru dengan mengukur Personal Learning Score (PLC). Nilai PLC dihitung setiap menit, bernilai sebanyak jumlah soal yang dikerjakan di menit tersebut. Nilai PLC akan diakumulasi selama L menit terakhir. Jika nilai akumulasi PLC selama L menit terakhir melebihi M, maka siswa tersebut akan mendapatkan 1 Piala.

Sebagai contoh, misal Andy belajar selama N menit dengan catatan berikut

Menit ke 1: 6 PLC
Menit ke 2: 0 PLC
Menit ke 3: 0 PLC
Menit ke 4: 1 PLC
Menit ke 5: 5 PLC
Menit ke 6: 1 PLC
Menit ke 7: 1 PLC
Menit ke 8: 0 PLC
Jika L adalah 7 dan M adalah 10

Di menit ke 1, akumulasi PLCnya 6. Belum mendapat piala.
Di menit ke 2, akumulasi PLCnya 6. Belum mendapat piala.
Di menit ke 3, akumulasi PLCnya 6. Belum mendapat piala.
Di menit ke 4, akumulasi PLCnya 7. Belum mendapat piala.
Di menit ke 5, akumulasi PLCnya 12. Mendapat 1 piala.
Di menit ke 6, akumulasi PLCnya 13. Mendapat 1 piala lagi.
Di menit ke 7, akumulasi PLCnya 14. Mendapat 1 piala lagi.
Di menit ke 8, akumulasi PLCnya 8 (penjumlahan 7 menit terakhir karena L = 7). Tidak mendapat piala.
Maka Andy mendapatkan total 3 piala.

Input
Baris pertama adalah T jumlah test cases, 1 <= T <= 10
T baris berikutnya berisi dua baris dengan format (space separated):
Baris pertama: L M N
1 <= M <= 10,000,000
1 <= L <= 10,000
Baris kedua: PLC[1] PLC[2] ... PLC[N]
PLC[i] adalah nilai PLC di menit ke i (1 <= i <= N)
0 <= PLC[i] <= 10
Test Set 1
1 <= N <= 1,000
Test Set 2
1,001 <= N <= 1,000,000
Output
Untuk masing-masing test case, print 1 baris dengan format Case #i: piala, di mana i adalah nomor test casenya (dimulai dari 1) dan piala adalah jumlah piala yang didapat
Sample Input
3
7 10 8
6 0 0 1 5 1 1 0
7 10 7
1 1 1 1 1 1 1
3 9 7
3 3 3 4 3 3 3
Sample Output
Case #1: 3
Case #2: 0
Case #3: 3
Explanation
Untuk Case #1, penjelasannya sesuai dengan di penjelasan soal di atas.

Answer Submission Instructions
There is small case and big case score, each has its max score like shown below, your task is to get the highest possible score.
Once you run your code, your source code, small case & big case output will be automatically saved as the answer.
You may run your code as many time as you want (as long as there's still time) until you get the highest possible score.
On some programming languages, we already provide you the template that read the input data, just click Insert Template from top left menu.
The total coding score that we will assess is the sum up of all small and big case scores across all coding tests.
Please make sure the content formatting (symbols, capitalization, space, line break, etc.) of the output result from your code
must match exactly the same like in the sample output shown on the question because it will affect your scoring if you miss even a single space.
Because the data on some small/big case input is huge, so the time to execute your code can be very long. We recommend you to run
the sample case first to make sure your code is right. Note that you will not get any score from sample case, it's just a playground.
You can also edit sample input data from the editor, in case you need to debug/test your code.
