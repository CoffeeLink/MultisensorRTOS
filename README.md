# MultisensorRTOS
Multi-sensor ultrasonik dengan implementasi RTOS

Nilai didalam fungsi vTaskDelay tergantung dari lama eksekusi task. Jauh jarak yang terdeteksi oleh sensor mempengaruhi waktu eksekusi task. Semakin jauh jarak yang terdeteksi maka semakin lama waktu eksekusi task tersebut. Sehingga nilai didalam fungsi vTaskDelay perlu untuk ditambah.

## References
- Septiawan, I., Akbar, S., & Syauqy, D. (2018). Rancang Bangun Sistem Multi-Sensor Untuk Pengukuran Jarak Secara Simultan. Jurnal Pengembangan Teknologi Informasi Dan Ilmu Komputer, 2(11), 5394-5401. Diambil dari http://j-ptiik.ub.ac.id/index.php/j-ptiik/article/view/3293 
