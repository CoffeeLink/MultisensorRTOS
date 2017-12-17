# MultisensorRTOS
Multi-sensor ultrasonik dengan implementasi RTOS

Nilai didalam fungsi vTaskDelay tergantung dari lama eksekusi task. Jauh jarak yang terdeteksi oleh sensor mempengaruhi waktu eksekusi task. Semakin jauh jarak yang terdeteksi maka semakin lama waktu eksekusi task tersebut. Sehingga nilai didalam fungsi vTaskDelay perlu untuk ditambah.



