<h2>Analisis Algoritma Berdasarkan Tiap Kasus</h2>

<h3>Algoritma Bubble Sort dan Insertion Sort</h3>
<ol>
  <li>
    <strong>Bubble Sort</strong>
    <ul>
      <li>Worst Case: Terjadi ketika array terurut secara terbalik. Setiap elemen harus ditukar dengan elemen di sebelahnya selama setiap iterasi. Kompleksitas waktu Bubble Sort dalam worst case adalah O(n^2), di mana n adalah jumlah elemen dalam array.</li>
      <li>Best Case: Terjadi ketika array sudah terurut secara terurut. Setelah satu iterasi, algoritma akan mengenali bahwa tidak ada pertukaran yang dilakukan. Kompleksitas waktu Bubble Sort dalam best case adalah O(n), karena setiap elemen hanya dibandingkan sekali.</li>
      <li>Average Case: Jika kita mengasumsikan bahwa input yang diberikan secara acak, kompleksitas waktu rata-rata Bubble Sort adalah O(n^2). Ini berarti algoritma akan membutuhkan waktu yang sebanding dengan jumlah elemen dalam array yang akan diurutkan.</li>
    </ul>
  </li>
  <li>
    <strong>Insertion Sort</strong>
    <ul>
      <li>Worst Case: Terjadi ketika array terurut secara terbalik dan setiap elemen harus dipindahkan ke posisi awal saat memasukkan elemen baru. Dalam kasus ini, kompleksitas waktu Insertion Sort dalam worst case juga adalah O(n^2).</li>
      <li>Best Case: Terjadi ketika array sudah terurut secara terurut. Dalam hal ini, setelah satu iterasi, algoritma hanya perlu membandingkan elemen terakhir dengan elemen sebelumnya, dan tidak ada pergeseran yang diperlukan. Kompleksitas waktu Insertion Sort dalam best case adalah O(n).</li>
      <li>Average Case: Rata-rata, algoritma Insertion Sort akan melakukan sekitar (n^2) / 4 perbandingan dan pemindahan. Waktu komputasi dalam average case juga adalah O(n^2).</li>
    </ul>
  </li>
</ol>

<h3>Algoritma TSP dan Dijkstra</h3>
<ol>
  <li>
    <strong>Analisis Travelling Salesman Problem (TSP)</strong>
    <ul>
      <li>Worst Case: Pada kasus terburuk, algoritma TSP akan mencoba semua kemungkinan permutasi jalur yang memenuhi kriteria awal dan tujuan. Jumlah simpul dalam grafik: n. Jumlah permutasi: (n-1)!. Dalam implementasi menggunakan fungsi itertools.permutations untuk menghasilkan semua permutasi jalur. Oleh karena itu, kompleksitas waktu algoritma TSP pada kasus terburuk adalah O((n-1)!).</li>
      <li>Best Case: Pada kasus terbaik, jika grafik hanya memiliki 2 simpul (misalnya 'a' dan 'b'), algoritma TSP akan langsung menemukan jalur terpendek tanpa perlu memeriksa banyak permutasi. Dalam implementasi jika hanya terdapat 2 simpul, algoritma TSP akan memeriksa satu jalur langsung dari simpul awal ke simpul tujuan. Sehingga, kompleksitas waktu algoritma TSP pada kasus terbaik adalah O(1).</li>
      <li>Average Case: Pada kasus rata-rata, kompleksitas waktu algoritma TSP dalam implementasi Anda tergantung pada jumlah simpul dalam grafik.  Dalam implementasi menggunakan itertools.permutations untuk menghasilkan semua permutasi jalur yang mungkin. Dalam implementasi ini, algoritma TSP akan mencoba setiap permutasi jalur yang memenuhi kriteria awal dan tujuan. Jumlah iterasi yang dilakukan dapat didekati sebagai faktorial dari jumlah simpul dikurangi dengan faktorial dari jumlah simpul dikurangi 1. Oleh karena itu, kompleksitas waktu algoritma TSP pada kasus rata-rata adalah O((n-1)!).</li>
    </ul>
  </li>
  <li>
    <strong>Analisis Dijkstra</strong>
    <ul>
      <li>Worst Case: Pada kasus terburuk, jika setiap simpul terhubung dengan semua simpul lainnya dalam grafik, kompleksitas waktu algoritma Dijkstra akan mencapai maksimum. Jumlah simpul dalam grafik: n. Jumlah tepi (edges) dalam grafik: m. Dalam implementasi, algoritma Dijkstra menggunakan struktur data heap biner untuk mengoptimalkan pemrosesan simpul dengan jarak terpendek. Algoritma Dijkstra akan memproses setiap simpul dan tepi dalam grafik, dengan jumlah iterasi sebanyak n * m. Oleh karena itu, kompleksitas waktu algoritma Dijkstra pada kasus terburuk adalah O(n * m).</li>
      <li>Best Case: Pada kasus terbaik, jika grafik hanya memiliki satu simpul, algoritma Dijkstra hanya akan memproses simpul tersebut. Dalam implementasi, jika hanya terdapat satu simpul, algoritma Dijkstra akan segera menyelesaikan dengan satu iterasi. Sehingga, kompleksitas waktu algoritma Dijkstra pada kasus terbaik adalah O(1).</li>
      <li>Average Case: Pada kasus rata-rata, kompleksitas waktu algoritma Dijkstra dalam implementasi Anda tergantung pada jumlah simpul dan tepi dalam grafik. Dalam implementasi ini, algoritma Dijkstra menggunakan struktur data heap biner untuk mengoptimalkan pemrosesan simpul dengan jarak terpendek. Jumlah iterasi yang dilakukan dapat bervariasi tergantung pada jumlah simpul dan tepi dalam grafik. Oleh karena itu, kompleksitas waktu algoritma Dijkstra pada kasus rata-rata adalah O(n * m).</li>
    </ul>
  </li>
</ol>
