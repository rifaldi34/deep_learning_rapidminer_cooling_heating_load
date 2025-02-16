# deep_learning_rapidminer_cooling_heating_load

![image](https://github.com/user-attachments/assets/ae551cc2-4df9-405f-8c4d-9433d1801ac4)

![image](https://github.com/user-attachments/assets/fd8cd907-862c-4660-b0ac-3f49930ed191)

Proyek ini bertujuan memprediksi beban pemanasan (Heating_Load) dan pendinginan (Cooling_Load) pada bangunan dengan menggunakan delapan fitur fisik sebagai input. Stakeholder yang berkepentingan meliputi perancang bangunan, insinyur energi, dan pengelola fasilitas yang membutuhkan estimasi kebutuhan energi secara akurat. Dataset yang digunakan berasal dari Kaggle https://www.kaggle.com/datasets/ujjwalchowdhury/energy-efficiency-data-set dengan 768 baris data, 8 fitur input, dan 2 target output.

Pada tahap persiapan data, dilakukan penetapan peran (role) dengan menetapkan variabel target sebagai label dan fitur-fitur lainnya sebagai input. Dataset asli diduplikasi agar setiap target (Heating_Load dan Cooling_Load) dapat diproses secara terpisah. Selanjutnya, data dibagi menjadi 80% data latih dan 20% data uji untuk masing-masing target guna memastikan setiap model dapat dilatih dan dievaluasi secara independen.

Modeling menggunakan algoritma deep learning, dimana model dilatih menggunakan data latih untuk mempelajari pola hubungan antara fitur dan target. Setelah proses pelatihan, model diuji menggunakan data uji yang belum pernah dilihat sebelumnya. Evaluasi model menggunakan metrik Root Mean Squared Error (RMSE), yang menghasilkan nilai RMSE sekitar 0.407 untuk Heating_Load dan 0.760 untuk Cooling_Load, menandakan bahwa prediksi untuk Heating_Load lebih akurat.

Pada tahap deployment, model yang telah terlatih diintegrasikan ke dalam simulator untuk menangani input parameter baru. Simulator ini memungkinkan prediksi secara real-time untuk kedua target, membantu perencanaan sistem pendingin dan pemanas yang lebih efisien serta mengurangi biaya operasional.
