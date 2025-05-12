## FigureGeneration
# FA_figuregeneration
Реализовать API, которое позволяет генерировать, преобразовывать и визуализировать последовательность плоских полигонов, представленных в виде картежа картежей (например: ((0,0), (0,1), (1,1), (1,0)) — представление для квадрата). Последовательности представлений полигонов представляют собой итераторы (далее: последовательности полигонов). Решать задачи с использованием функционального стиля программирования, в том числе активно использовать функции из модуля itertools и functools.


<img width="582" alt="image" src="https://github.com/user-attachments/assets/dd3f893d-cd1c-44aa-bd0f-daa703a70343" />

Реализовать функции, генерирующие бесконечную последовательность непересекающихся полигонов с различающимися координатами (например, «ленту», см. рис. 2):
прямоугольников (gen_rectangle);



<img width="577" alt="image" src="https://github.com/user-attachments/assets/fff1e0f6-6143-416d-ad04-16fe3faa5d42" />


треугольников (gen_triangle);


<img width="625" alt="image" src="https://github.com/user-attachments/assets/f4622f41-8681-415a-9bda-5d29c4468625" />


правильных шестиугольников (gen_hexagon).



<img width="1136" alt="image" src="https://github.com/user-attachments/assets/9ee370a2-6627-4523-936f-8889c3ecc15a" />



с помощью данных функций используя функции из модуля itertools сгенерировать семь фигур, включающих как прямоугольники, так и треугольники и шестиугольники, визуализировать результат.






Реализовать операции:


параллельный перенос
 (tr_translate);

 <img width="598" alt="image" src="https://github.com/user-attachments/assets/a91553ae-4c00-4734-b078-ec84b2b884a0" />


поворот (tr_rotate);


<img width="611" alt="image" src="https://github.com/user-attachments/assets/e6e25e26-13bf-4489-9f8e-31bdc46e62e0" />


симметрия (tr_symmetry);

<img width="601" alt="image" src="https://github.com/user-attachments/assets/3179f43a-add5-4a9f-b373-720921093dcc" />


гомотетия (tr_homothety);



<img width="605" alt="image" src="https://github.com/user-attachments/assets/18a3bd03-ddae-4ff3-89e4-db27cf281f7e" />

которые можно применить к последовательности полигонов с помощью функции map.

